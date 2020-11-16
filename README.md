# How to edit the website

## Projects

Don't edit any html directly. Instead, modify projects.xml

Each project entry should have the following format:
```
  <project>
    <title>title of the project</title>
    <description>very very short description (~3 words)</description>
    <blurb>longer blurb for project page</blurb>
    <img>background image covering the link</img>
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

## Publications

Don't edit any html directly. Instead, modify publications.xml

Publications will automatically populate the project and papers pages from here. Each publication entry should have the following format:
```
  <publication>
    <project>Project name to filter under, which much be present in projects.xml</project>
    <title>Title of the paper</title>
    <url>Url to the paper</url>
    <codeurl>Url to paper code (optional)</codeurl>
    <dataurl>Url to paper data (optional)</dataurl>
    <authors>First Last, First Last, etc</authors>
    <conference>Conference name, e.g. ACL</conference>
    <year>Year of publication, e.g. 2030</year>
  </publication>
```

## Adding new pages
To add new pages, copy and modify template.html, which will automatically have bootstrap formatting.

Then, add a link to index.html, e.g.:
```
  <li><a href="#" class="nav-link" data-url="mypage.html">My Page</a></li>
```
modifying "mypage.html" to the page name. It should work automatically in the navigation.
