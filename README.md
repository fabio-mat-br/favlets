# favlets


## Limpar cookies e localStorage



`javascript:(function(){window.localStorage.clear();document.cookie.split(";").forEach(function(c) { document.cookie = c.replace(/^ +/, "").replace(/=.*/, "=;expires=" + new Date().toUTCString() + ";path=/"); }); })();`



## Parâmetros da URL 

`javascript:void(window.location.href.split('?')[1].split('&').forEach(e =>{ console.log(e.split('=')) }))`



## Query string de qualquer URL (num prompt)

`javascript:void(prompt('Coloque a URL').split('?')[1].split('&').forEach(e =>{ console.log(decodeURIComponent(e).split('=')) }))`



## Exibição dos `ids` da página

`javascript:var nodesArray = [].slice.call(document.querySelectorAll("[id]"));nodesArray.forEach(e => {e.style.border='solid 1px red';var newE = document.createElement('span');newE.style.background = '#FFCC00';newE.style.padding = '3px';newE.style.border = 'solid 1px blue';var nodeT = document.createTextNode(e.getAttribute('id'));newE.appendChild(nodeT);e.parentNode.insertBefore(newE, e.nextSibling);})` 



## Selector gadget

`javascript:(function(){var s=document.createElement('div');s.innerHTML='Loading...';s.style.color='black';s.style.padding='20px';s.style.position='fixed';s.style.zIndex='9999';s.style.fontSize='3.0em';s.style.border='2px solid black';s.style.right='40px';s.style.top='40px';s.setAttribute('class','selector_gadget_loading');s.style.background='white';document.body.appendChild(s);s=document.createElement('script');s.setAttribute('type','text/javascript');s.setAttribute('src','https://dv0akt2986vzh.cloudfront.net/unstable/lib/selectorgadget.js');document.body.appendChild(s);})();`

 
