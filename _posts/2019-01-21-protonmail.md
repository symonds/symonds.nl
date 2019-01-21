---
layout: post
comments: true
title: ProtonMail Themes
excerpt_separator: <!-- more -->
---

This weekend I read a reddit post about theming ProtonMail with a little bit of CSS and the built in themes

<!-- more -->


This section expands the left hand navigation pane, which has all the folders/lables listed

I wanted this to be wider so that it didn't truncate my folder names.
```
.headerSecuredDesktop-logo {
    width: 250px;
}

body #ptSidebar {
    width: 250px;
}

body #pm_main {
    width: calc(100% - 250px);
}
```

This section changes the height of the folders/lables scrollbox on the top bar.
```
.scrollbox-container {
    max-height: 500px;
}
```

This section was stolen from [Here](https://austingwalters.com/protonmail-css-theme/) and shrinks the conversation pane.
```
#pm_view {
  min-width:70%;
}

#conversation-list-columns{
  border-right:none;
  background:#F7F6F6;
  max-width:30%;
}

#conversation-view{
  min-width:68%;
}
```
