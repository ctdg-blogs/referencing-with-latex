#### VS code 
 settings of extension `latex workshop`

---
#### Find Settings.json
File > Prefferences > Settings
enter search settings editview: `latex workshop`
find the link on result page: `Edit in settings.json`

---
#### Edit settings.json
```json
"latex-workshop.latex.tools": [
	    {
	        "name": "xelatex",
	        "command": "xelatex",
	        "args": [
	          "-synctex=1",
	          "-interaction=nonstopmode",
	          "-file-line-error",
	          "%DOC%"
        	]
        },
		{
	        "name": "pdflatex",
	        "command": "pdflatex",
	        "args": [
	          "-synctex=1",
	          "-interaction=nonstopmode",
	          "-file-line-error",
	          "%DOC%"
	        ]
	    },
	    {
	        "name": "bibtex",
	        "command": "bibtex",
	        "args": [
	          "%DOCFILE%"
	    	]
	    }
	],
```