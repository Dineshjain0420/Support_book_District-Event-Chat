## Search for Content

<input type="text" id="search" onkeyup="searchFunction()" placeholder="Search for links or content...">

<ul id="content-list">
  
  ## <span style="color: Green;">Documents Links</span> 📚

  ### General Links 🌐
  <li><a href="https://docs.google.com/spreadsheets/d/1it4rlECHXYQtrjr24LQ3MzIkkOjy9dFdY92cCe201IE/edit?gid=89651715#gid=89651715" target="_blank">District Event Details</a> 📊</li>
  <li><a href="https://docs.google.com/spreadsheets/d/1awPy28Dw_jGX907CiAoTCtIGIYg0iKshfoMxRAQqUKw/edit?gid=1594796217#gid=1594796217" target="_blank">EVENTS UPDATES</a> 🔄</li>

  ### Specific Event Links 🎤
  <li><a href="https://docs.google.com/spreadsheets/d/1VRpi0APPkfQSWJzBhfIyNAqn1e5GEWUTxmp8qhtvSg4/edit?gid=54208201#gid=54208201" target="_blank">Honey Singh Updates</a> 🎶</li>
  <li><a href="https://docs.google.com/spreadsheets/d/11arNieLnwollg3r4o6xYrNxvAIcT3HIXNC_o-MdRJVQ/edit?gid=307067024#gid=307067024" target="_blank">INDvsENG FAQs All Cities</a> 🏏</li>
  <li><a href="https://docs.google.com/spreadsheets/d/1xygjFsQGanMbqV9AmID3JS-j7QOY7WfhNwPXvKxulg4/edit?gid=0#gid=0" target="_blank">Arijit Singh Live Pune FAQs Jan 16-5 PM</a> 🎤</li>

  ## <span style="color: Green;">Important Web Links</span> 🌍
  <li><a href="https://external.zomans.com/support/agent" target="_blank">Chat App</a> 💬</li>
  <li><a href="https://insider.in" target="_blank">Insider</a> 🔍</li>
  <li><a href="https://admin.insider.in" target="_blank">Insider Login</a> 🔑</li>
  <li><a href="https://insider.in/zomaland-by-zomato-carnival/article" target="_blank">Zomaland</a> 🎉</li>
  <li><a href="https://docs.google.com/forms/u/0/d/e/1FAIpQLScozlEwq8q4piV1PoflZOyTkBQlsTp0NCd_HS_y69xCVBHgXQ/formResponse" target="_blank">Refund Form</a> 📝</li>
  <li><a href="https://www.zomato.com/" target="_blank">Zomato</a> 🍴</li>
  <li><a href="https://external.zomans.com/" target="_blank">External Zomans</a> 🔗</li>
  <li><a href="https://external-access.zomans.com/#/apps" target="_blank">Lifeline Profile</a> 🏥</li>
  <li><a href="https://web.whatsapp.com/" target="_blank">WhatsApp Web</a> 💬</li>

  ## Useful Tools
  <li><a href="https://chromewebstore.google.com/detail/quillbot-ai-writing-and-g/iidnbdjijdkbmajdffnidomddglmieko?hl=en-US&utm_source=quillbot.com&utm_medium=referral&utm_campaign=extension_landing_page&utm_content=fixed_banner&utm_term=direct" target="_blank">QuillBot Chrome Extension</a></li>
  <li><a href="https://chromewebstore.google.com/detail/grammarly-ai-writing-and/kbfnbcaeplbcioakkpcpgfkobkghlhen?hl=en" target="_blank">Grammarly Chrome Extension</a></li>
  <li><a href="https://chromewebstore.google.com/detail/volume-master/jghecgabfgfdldnmbfkhmffcabddioke" target="_blank">Volume Master Chrome Extension</a></li>

  ## Download / Activate Office 💻
  ### Download Office 365 Pro Plus 🔽
  <li><a href="https://c2rsetup.officeapps.live.com/c2r/download.aspx?ProductreleaseID=O365ProPlusRetail&platform=x64&language=en-us&version=O16GA" target="_blank">Download Office 365 Pro Plus</a></li>

  ### For Windows & Office Activation ⚙️
  <li>
      1. On **Windows 10/11**, right-click on the **Windows Start menu**, and select **PowerShell** or **Terminal**.
      2. Copy-paste the below code and press **Enter**:
      ```powershell
      irm https://get.activated.win | iex
      ```
      3. You will see the activation options, follow the onscreen instructions.
  </li>
  
</ul>

# _Thank You!_ 😊

<script>
function searchFunction() {
    let input = document.getElementById('search');
    let filter = input.value.toLowerCase();
    let ul = document.getElementById("content-list");
    let li = ul.getElementsByTagName('li');

    for (let i = 0; i < li.length; i++) {
        let a = li[i].getElementsByTagName("a")[0];
        if (a.innerHTML.toLowerCase().indexOf(filter) > -1) {
            li[i].style.display = "";
        } else {
            li[i].style.display = "none";
        }
    }
}
</script>




