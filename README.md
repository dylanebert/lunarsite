# How to edit the website

## Projects

Don't edit any html directly. Instead, modify projects.xml

Each project entry should have the following format:
```
  <project>
    <title>title of the project</title>
    <description>very very short description (~3 words)</description>
    <img>background image covering the link</img>
    <url>link to the project site (optional)</url>
  </project>
```

## People

Don't edit any html directly. Instead, modify people.xml

Each person entry should have the following format, and be placed under either <current> or <past> appropriately:
```
  <person>
    <name>Firstname Lastname</name>
    <status>Ph.D., Masters, etc.</status>
    <img>Link to picture of the person (optional, requires description)</img>
    <description>Description of the person's work (optional, requires img)</description>
    <url>Link to person's external website (optional)</url>
  </person>
```
  
## Adding new pages
To add new pages, copy and modify template.html, which will automatically have bootstrap formatting. 

Then, add a link to index.html, e.g.:
```
  <li><a href="#" class="nav-link" data-url="mypage.html">My Page</a></li>
```
modifying "mypage.html" to the page name. It should work automatically in the navigation.
