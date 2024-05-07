---
layout: default
---

<style>
.tablinks {
  background-color: #2A3132;
  color: white;
  border: none;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  transition-duration: 0.4s;
  border-radius: 12px; /* This makes the button corners rounded */
}

.tablinks:hover {
  background-color: #336B87;
}
</style>

# Text

This is the text page.

<button class="tablinks"><a href="{{ site.baseurl }}/index">Home</a></button>
<button class="tablinks"><a href="{{ site.baseurl }}/data">Data</a></button>
<button class="tablinks"><a href="{{ site.baseurl }}/network">Network</a></button>