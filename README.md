## Plant search bookmarklets

The following links are 'bookmarklets' – links allow you to search BBG's plant records via the its public website. You can search in two ways: by highlighting a plant name or accession number in your web browser and clicking the bookmarklets in your bookmarks bar; or by clicking the bookmarklets first and entering a plant details in the on-screen prompt.

Further details are in the main GitHub repository [here](https://github.com/rowanblaik/plant-search-bookmarklets).

### How to install

Make sure your web browser's bookmarks bar is visible and drag each of the following three links to it:

|Link|Search by|
|------|-----------------|
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter an accession number:',''))};Qr=Qr.replace(/(?!^x)\D/gi,'');if(Qr)window.open('https://www.bbg.org/cgi/plant-records/detail.cgi?'+encodeURIComponent(Qr),'_blank');">BBG acc#</a>| accession number |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name (wildcard=*):',''))};if(Qr)window.open('https://www.bbg.org/cgi/plant-records/search.cgi?name='+encodeURIComponent(Qr),'_blank');">BBG name</a>| scientific name |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a common plant name (wildcard=*):',''))};if(Qr)window.open('https://www.bbg.org/cgi/plant-records/search_advanced.cgi?com_name='+encodeURIComponent(Qr),'_blank');">BBG com</a>| common name |

### To test your installation

Highlight the following plant name: _Magnolia_ × _brooklynensis_ and click the "BBG name" bookmark.

### Other plant databases

|Link|Search by|
|------|-----------------|
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('http://www.worldfloraonline.org/search?query='+encodeURIComponent(Qr),'_blank');">WFO</a>| World Flora Online |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x \| × /g,' ');if(Qr)window.open('http://www.theplantlist.org/tpl1.1/search?q='+encodeURIComponent(Qr),'_blank');">TPL</a>| The Plant List |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('https://www.rhs.org.uk/Plants/Search-Results?query='+encodeURIComponent(Qr),'_blank');">RHS-PF</a>| RHS \'Find a plant\' |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/×/g,'').replace(/['‘’]/g,'').replace(/\s+/g,' and ');if(Qr)window.open('http://apps.rhs.org.uk/horticulturaldatabase/summary2.asp?crit='+encodeURIComponent(Qr)+'&genus='+Qr.match(/\w+/),'_blank');">RHS-DB</a>| RHS \'Hort DB\' |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('http://www.missouribotanicalgarden.org/PlantFinder/PlantFinderProfileResults.aspx?adv='+encodeURIComponent(Qr),'_blank');">MBG</a>| Mobot Plant Finder |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x \| × /g,' ×');if(Qr)window.open('http://plants.usda.gov/java/nameSearch?mode=sciname&keywordquery='+encodeURIComponent(Qr),'_blank');">USDA-P</a>| USDA PLANTS database |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};if(Qr)window.open('https://garden.org/plants/search/text/?q='+encodeURIComponent(Qr),'_blank');">NGA-DB</a>| NGA plants database |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/×/g,'x');if(Qr)window.open('http://pfaf.org/user/Plant.aspx?LatinName='+encodeURIComponent(Qr),'_blank');">PFAF</a>| Plants for a Future |
|<a href="javascript:Qr=document.getSelection().toString().trim();if(Qr==''){void(Qr=window.prompt('Enter a scientific plant name:',''))};Qr=Qr.replace(/ x \| × /g,' ×');if(Qr)window.open('http://newyork.plantatlas.usf.edu/Results.aspx?q='+encodeURIComponent(Qr),'_blank');">NYFA</a>| New York Flora Atlas |

### Credits

This bookmarklets were inspired by RBG Kew's ePIC [browser button](http://epic.kew.org/tbutton.htm).
