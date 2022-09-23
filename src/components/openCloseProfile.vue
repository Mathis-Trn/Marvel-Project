<script>
    function openCloseProfile(div)
{
var profile = document.getElementsByClassName("profileContent");
var profile_clic = div.querySelector(".profileContent");
for (var i = 0, numbers = profile.length; i < numbers; i++)
{
   if ((profile[i].classList.contains("visible") == true) && (profile[i] != profile_clic))
   {
   profile[i].classList.remove ('visible');
   profile[i].classList.toggle ('hidden');
   }
}
var divContent = div.getElementsByTagName('div')[1];
if (divContent.classList.contains("hidden") == true) 
{
   divContent.classList.remove ('hidden');
   divContent.classList.toggle ('visible');
}
else if (divContent.classList.contains("visible") == true) 
{
   divContent.classList.remove ('visible');
   divContent.classList.toggle ('hidden');
}
}
</script>