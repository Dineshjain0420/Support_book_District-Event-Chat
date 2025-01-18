## <span style="color: Green;">Documents Links</span> 📚

### General Links 🌐

- <a href="https://docs.google.com/spreadsheets/d/1it4rlECHXYQtrjr24LQ3MzIkkOjy9dFdY92cCe201IE/edit?gid=89651715#gid=89651715" target="_blank">District Event Details</a> 📊
- <a href="https://docs.google.com/spreadsheets/d/1awPy28Dw_jGX907CiAoTCtIGIYg0iKshfoMxRAQqUKw/edit?gid=1594796217#gid=1594796217" target="_blank">EVENTS UPDATES</a> 🔄

### Specific Event Links 🎤

- <a href="https://docs.google.com/spreadsheets/d/1VRpi0APPkfQSWJzBhfIyNAqn1e5GEWUTxmp8qhtvSg4/edit?gid=54208201#gid=54208201" target="_blank">Honey Singh Updates</a> 🎶
- <a href="https://docs.google.com/spreadsheets/d/11arNieLnwollg3r4o6xYrNxvAIcT3HIXNC_o-MdRJVQ/edit?gid=307067024#gid=307067024" target="_blank">INDvsENG FAQs All Cities</a> 🏏
- <a href="https://docs.google.com/spreadsheets/d/1xygjFsQGanMbqV9AmID3JS-j7QOY7WfhNwPXvKxulg4/edit?gid=0#gid=0" target="_blank">Arijit Singh Live Pune FAQs Jan 16-5 PM</a> 🎤

## <span style="color: Green;">Important Web Links</span> 🌍

- <a href="https://external.zomans.com/support/agent" target="_blank">Chat App</a> 💬 - <a href="https://insider.in" target="_blank">Insider</a> 🔍 - <a href="https://admin.insider.in" target="_blank">Insider Login</a> 🔑 - <a href="https://insider.in/zomaland-by-zomato-carnival/article" target="_blank">Zomaland</a> 🎉 - <a href="https://docs.google.com/forms/u/0/d/e/1FAIpQLScozlEwq8q4piV1PoflZOyTkBQlsTp0NCd_HS_y69xCVBHgXQ/formResponse" target="_blank">Refund Form</a> 📝  
- <a href="https://www.zomato.com/" target="_blank">Zomato</a> 🍴 - <a href="https://external.zomans.com/" target="_blank">External Zomans</a> 🔗 - <a href="https://external-access.zomans.com/#/apps" target="_blank">Lifeline Profile</a> 🏥 - <a href="https://web.whatsapp.com/" target="_blank">WhatsApp Web</a> 💬

## Useful Tools

##### QuillBot ✍️ - <a href="https://chromewebstore.google.com/detail/quillbot-ai-writing-and-g/iidnbdjijdkbmajdffnidomddglmieko?hl=en-US&utm_source=quillbot.com&utm_medium=referral&utm_campaign=extension_landing_page&utm_content=fixed_banner&utm_term=direct" target="_blank">QuillBot Chrome Extension</a>

##### Grammarly 📝 - <a href="https://chromewebstore.google.com/detail/grammarly-ai-writing-and/kbfnbcaeplbcioakkpcpgfkobkghlhen?hl=en" target="_blank">Grammarly Chrome Extension</a>

##### Volume Master 🔊 - <a href="https://chromewebstore.google.com/detail/volume-master/jghecgabfgfdldnmbfkhmffcabddioke" target="_blank">Volume Master Chrome Extension</a>

## Download / Activate Office 💻

### Download Office 365 Pro Plus 🔽

- <a href="https://c2rsetup.officeapps.live.com/c2r/download.aspx?ProductreleaseID=O365ProPlusRetail&platform=x64&language=en-us&version=O16GA" target="_blank">Download Office 365 Pro Plus</a>

### For Windows & Office Activation ⚙️

1. On **Windows 10/11**, right-click on the **Windows Start menu**, and select **PowerShell** or **Terminal**.

2. Copy-paste the below code and press **Enter**:

    ```powershell
    irm https://get.activated.win | iex
    ```

3. You will see the activation options, follow the onscreen instructions.


# _Thank You!_ 😊






<script type="text/hoplon">
(page "index.html")

(defn mouse-loc->vec
  "Given a Google Closure normalized DOM mouse event return the
  mouse x and y position as a two element vector."
  [e]
  [(.-clientX e) (.-clientY e)])

;; =============================================================================
;; Example 1

(defc ex1-content         ["Waiting for a click ...."])
(defc ex1-click-count     0)
(defn ex1 []
  (when (< @ex1-click-count 1)
    (swap! ex1-click-count inc)
    (swap! ex1-content conj "Got a click!")))

;; =============================================================================
;; Example 2

(defc ex2-content         ["Waiting for a click ...."])
(defc ex2-click-count     0)
(defn ex2 []
  (when (= @ex2-click-count 1)
    (swap! ex2-click-count inc)
    (swap! ex2-content conj "Done"))
  (when (= @ex2-click-count 0)
    (swap! ex2-click-count inc)
    (swap! ex2-content conj "Got a Click!" "Waiting for another click ....")))  

;; =============================================================================
;; Example 3

(defc ex3-content           ["Waiting for a click from Button A ....."])
(defc ex3-click-count-a     0)
(defc ex3-click-count-b     0)
(defn ex3a []
  (when (= @ex3-click-count-a 0)
    (swap! ex3-click-count-a inc)
    (swap! ex3-content conj "Got a click!" "Waiting for a click from Button B ....")) )
(defn ex3b []
  (when (and (= @ex3-click-count-a 1) (= @ex3-click-count-b 0))
    (swap! ex3-click-count-b inc)
    (swap! ex3-content conj "Done!")))

;; =============================================================================
;; Example 6

(defc ex6-content           ["Click the button to start tracking the mouse."])
(defc ex6-button-name       "GO!")
(defn ex6-toggle []
  (let [new-name    (if (= @ex6-button-name "GO!") "STOP!" "GO!")]
    (reset! ex6-button-name new-name)))
(defn ex6 [e]
  (when (= @ex6-button-name "STOP!")
    (swap! ex6-content conj (str (mouse-loc->vec e)))))

;; =============================================================================
;; Example 7

(defc ex7-content         ["Click the button to start tracking the mouse."])
(defc ex7-button-name     "GO!")
(defn ex7-toggle []
  (let [new-name    (if (= @ex7-button-name "GO!") "STOP!" "GO!")]
    (reset! ex7-button-name new-name)))
(defn ex7 [e]
  (when (= @ex7-button-name "STOP!")
    (let [[x y :as  m]   (mouse-loc->vec e)]
      (when (zero? (mod y 5))
        (swap! ex7-content conj (str m))))))

;; =============================================================================
;; Example 8

(defc ex8-content       ["Click the button ten times."])
(defc ex8-click-count   0)
(defn ex8 []
  (when (< @ex8-click-count 10)
    (swap! ex8-click-count inc)
    (when (= @ex8-click-count 1)
      (swap! ex8-content conj "1 Click!"))
    (when (> @ex8-click-count 1)
      (swap! ex8-content conj (str @ex8-click-count " clicks!")))
    (when (= @ex8-click-count 10)
      (swap! ex8-content conj "Done."))))

;; =============================================================================
;; Example 9

(defc ex9-index       0)
(defc ex9-animals     [:aardvark :beetle :cat :dog :elk :ferret
                     :goose :hippo :ibis :jellyfish :kangaroo])
(defc= ex9-card           (nth ex9-animals ex9-index))
(defn ex9-prev []
  (when (> @ex9-index 0)
    (swap! ex9-index dec)))
(defn ex9-next []
  (when (< @ex9-index (dec (count @ex9-animals)))
    (swap! ex9-index inc)))

;; =============================================================================
;; Example 10

(defc ex10-button-name  "START!")
(defc ex10-index       0)
(defn ex10 []
  (let [the-name    @ex10-button-name]
  (when (= the-name"START!")
    (reset! ex10-button-name "STOP!"))
  (when (= the-name"STOP!")
    (reset! ex10-button-name "DONE!"))))
(defc ex10-animals     [:aardvark :beetle :cat :dog :elk :ferret
                     :goose :hippo :ibis :jellyfish :kangaroo])
(defc= ex10-max        (dec (count ex10-animals)))
(defc= ex10-card           (nth ex10-animals ex10-index))
(defn ex10-prev []
  (if (> @ex10-index 0)
    (swap! ex10-index dec)
    (reset! ex10-index @ex10-max)))
(defn ex10-next []
  (if (< @ex10-index @ex10-max)
    (swap! ex10-index inc)
    (reset! ex10-index 0)))
(defn ex10-nav [k]
  (when (= @ex10-button-name "STOP!")
    (when (= k :next)
      (ex10-next))
    (when (= k :prev)
      (ex10-prev))))

(defn ex10-keys [e]
  (when (= @ex10-button-name "STOP!")
    (if (= (.-keyCode e) 39) (ex10-nav :next))
    (if (= (.-keyCode e) 37) (ex10-nav :prev))
    )
  )
</script>

<html>
    <head>
        <link rel="stylesheet" type="text/css" href="css/main.css" />
    </head>
    <body>
        <!-- Example 1 -->
        <div id="ex1" class="example">
            <h2>Example 1</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex1-button" on-click='{{ #(ex1) }}'>Click me</button>
                    </td>
                    <td id="ex1-display" class="display">
                        <div id="ex1-messages">
                        <loop-tpl bindings='{{ [x ex1-content] }}'>
                          <p><text>~{x}</text></p>
                        </loop-tpl>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 2 -->
        <div id="ex2" class="example">
            <h2>Example 2</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex2-button" on-click='{{ #(ex2) }}'>Click me</button>
                    </td>
                    <td id="ex2-display" class="display">
                        <div id="ex2-messages">
                        <loop-tpl bindings='{{ [x ex2-content] }}'>
                          <p><text>~{x}</text></p>
                        </loop-tpl>
                        </div>
                    </td>
                </tr>
            </table>
        </div>
        
        <!-- Example 3 -->
        <div id="ex3" class="example">
            <h2>Example 3</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex3-button-a" on-click='{{ #(ex3a) }}'>Button A</button>
                        <button id="ex3-button-b" on-click='{{ #(ex3b) }}'>Button B</button>
                    </td>
                    <td id="ex3-display" class="display">
                        <div id="ex3-messages">
                        <loop-tpl bindings='{{ [x ex3-content] }}'>
                          <p><text>~{x}</text></p>
                        </loop-tpl>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 4 -->
        <div id="ex4" class="example">
            <h2>Example 4</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex4-button-a">Go!</button>
                    </td>
                    <td id="ex4-display" class="display">
                        <div id="ex4-messages"></div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 5 -->
        <div id="ex5" class="example">
            <h2>Example 5</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex5-button">Go!</button>
                    </td>
                    <td id="ex5-display" class="display">
                        <div id="ex5-messages"></div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 6 -->
        <div id="ex6" class="example" on-mousemove='{{ #(ex6 %) }}' >
            <h2>Example 6</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex6-button" do-text='{{ ex6-button-name }}' on-click='{{ #(ex6-toggle)}}' ></button>
                    </td>
                    <td id="ex6-display" class="display">
                        <div class="scrolling">
                            <div id="ex6-messages">
                            <loop-tpl bindings='{{ [x ex6-content] }}'>
                              <p><text>~{x}</text></p>
                            </loop-tpl>
                            </div>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 7 -->
        <div id="ex7" class="example" on-mousemove='{{ #(ex7 %) }}'>
            <h2>Example 7</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex7-button" do-text='{{ ex7-button-name }}' on-click='{{ #(ex7-toggle)}}'></button>
                    </td>
                    <td id="ex7-display" class="display">
                        <div class="scrolling">
                            <div id="ex7-messages">
                            <loop-tpl bindings='{{ [x ex7-content] }}'>
                              <p><text>~{x}</text></p>
                            </loop-tpl>
                            </div>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 8 -->
        <div id="ex8" class="example">
            <h2>Example 8</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex8-button" on-click='{{ #(ex8) }}'>Click me!</button>
                    </td>
                    <td id="ex8-display" class="display card">
                        <div class="scrolling">
                            <div id="ex8-messages">
                            <loop-tpl bindings='{{ [x ex8-content] }}'>
                              <p><text>~{x}</text></p>
                            </loop-tpl>
                            </div>
                        </div>
                    </td>
                </tr>
            </table>
        </div>

        <!-- Example 9 -->
        <div id="ex9" class="example">
            <h2>Example 9</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex9-button-prev" on-click='{{ #(ex9-prev) }}' do-class='{{ (cell= {:disabled (= ex9-index 0)})}}'>Previous</button>
                        <button id="ex9-button-next" on-click='{{ #(ex9-next) }}' do-class='{{ (cell= {:disabled (= ex9-index (dec (count ex9-animals)))}) }}'>Next</button>
                    </td>
                    <td id="ex9-card" class="display card" do-text='{{ ex9-card }}'></td>
                </tr>
            </table>
        </div>

        <!-- Example 10 -->
        <div id="ex10" class="example" on-keydown='{{ #(ex10-keys %) }}'>
            <h2>Example 10</h2>
            <table>
                <tr>
                    <td class="left">
                        <button id="ex10-button-start-stop" do-text='{{ ex10-button-name}}' on-click='{{ #(ex10) }}'></button>
                        <button id="ex10-button-prev" on-click='{{ #(ex10-nav :prev) }}' 
                          do-class='{{ (cell= {:disabled (not= ex10-button-name "STOP!")}) }}'>Previous
                        </button>
                        <button id="ex10-button-next" on-click='{{ #(ex10-nav :next) }}' do-class='{{ (cell= {:disabled (not= ex10-button-name "STOP!")}) }}'>Next</button>
                    </td>
                    <td id="ex10-card" class="display card" do-text='{{ ex10-card }}'></td>
                </tr>
            </table>
        </div>
    </body>
</html>
