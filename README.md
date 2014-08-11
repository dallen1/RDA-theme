<h2>Introduction</h2>

<p>This is a guide for how the herring cove theme was applied. It assumes a basic understanding of css, the Jekyll manual for applying themes, and that the Herring Cove readme have been read.</p>

<h2>Theme application</h2>

<p>The following steps are getting the Herring Cove theme to apply to Metadata. This does not affect the navigation menus or homepage content.</p>
<p>
<ul>
<li>Fork metadata</li>
<li>Fork herring cove</li>
<li>Copy herring cove onto metadata</li>
  <ul>
    <li>_include/footer.html and _config.yml need to have data merged</li>
  </ul>
<li>Update index.md and add.md files in the following directories to use “about” or “links” layout</li>
  <ul>
    <li>/standards/</li>
    <li>/extensions/</li>
    <li>/subjects/</li>
    <li>/tools/</li>
    <li>/use_cases/</li>
  </ul>
<li>Convert current homepage to an “about” page and apply about theme.</li>
  <ul>
    <li>mkdir about</li>
    <li>cp index.md about/</li>
  </ul>
<li>Strip index.md of all content except for the layout tag.</li>
</ul>
</p>

<h2>Basic theme customization</h2>

<p>These steps will update the navigation bar and homepage text.</p>
<p>
<ul>
<li>Create navigation links for both the top bar and the side bar link lists.</li>
  <ul>
    <li>File location: “/_includes/header.html”</li>
  </ul>
<li>Update the homepage text to match the Metadata standards description on https://rd-alliance.org/</li>
  <ul>
    <li>File location: “/_includes/greeting.html” </li>
  </ul>
<li>Update the text overlay on the homepage image</li>
  <ul>
    <li>File location: “/_includes/showcase.html” </li>
  </ul>
<li>Change the picture for showcase</li>
  <ul>
    <li>Using a photo editor, change the stock photo to have the rda logo banner on the top. </li>
    <li>Image file location: /images</li>
    <li>Html file location: /_includes/showcase.html</li>
  </ul>
<li>Change the default theme title</li>
  <ul>
    <li>File location: “/_layouts/default.html”</li>
  </ul>
</ul>
</p>

<h2>Advanced theme customization</h2>

<p>The steps outlined below are for adjusting the size of the homepage image and homepage text.</p>

<p>
<ul>
<li>Change the font for the welcome text on the homepage.
  <ul>
    <li>File location: “/css/hc.css”</li>
    <li>Classes modified:</li>
      <ul>
        <li>#welcome-greeting > h1</li>
        <li>#welcome-greeting h1:hover</li>
        <li>#welcome-greeting > h2</li>
        <li>#welcome-greeting h2 a</li>
      </ul>
  </ul>
<li>Change the size of the photo</li>
  <ul>
    <li>File location: “/css/hc.css”</li>
    <li>Classes modified:</li>
      <ul>
        <li>.showcase-wrapper</li>
      </ul>
  </ul>
</ul>
</p>

