---
permalink: /index.html
markdown_extensions:
  - markdown_fenced_code_tabs
---
# code-snippets

<h1>Test</h1>

``` python fct_label="Python 2"
print "Bonjour" 
```


```javascript
  authenticate = () => {
          let address = "https://oauth.nzpost.co.nz/as/token.oauth2";
          let id = {client_id};
          let secret = {client_secret};
          let grant_type = "client_credentials";
          
          fetch(
            `${address}?grant_type=${grant_type}&client_id=${id}&client_secret=${secret}`,
            { method: "POST" }
          )
            .then(response => {
              if (response.status >= 200 && response.status <= 300) {
                response.json().then(json => {
                  // Do something with JSON
                });
              } else {
                // Handle error
              }
            })
            .catch(error => console.log("Error", error));
          });
        }


```
