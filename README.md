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

to edit people, edit people.xml

place each person element under the correct tag {faculty, current, past}
each person element requires:
<name>Firstname Lastname</name>
<status>phd, masters, etc</status>

and should optionally contain
<img>picture of the person</img>
<description>description of the person's work</description>
<url>link to person's external website</url>

img/description won't show up on the website unless the entry has BOTH
