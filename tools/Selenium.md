# Selenium

Although it's not the official documentation, Baiju Muthukadan's [Selenium with Python docs](http://selenium-python.readthedocs.org/en/latest/index.html) provide a great overview of the available methods in Selenium for Python. If that fails you, consult the [official documentation](http://docs.seleniumhq.org/docs/03_webdriver.jsp).

### Imports

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>from selenium import webdriver</code></td>
            <td>Imports access to the <a href="http://selenium-python.readthedocs.org/en/latest/api.html">Selenium Webdriver API</a>.</td>
        </tr>
    </tbody>
</table>

### Browser-Specific Commands

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>webdriver.Firefox()</code></td>
            <td>Use Selenium Webdriver to start a Firefox instance.</td>
        </tr>
        <tr>
            <td><code>webdriver.Firefox().get(url)</code></td>
            <td>Navigate to a specific URL. In the book, <code>webdriver.Firefox()</code> is assigned to a variable called <code>browser</code>, so that we can simply call <code>browser.get(url)</code>.</td>
        </tr>
        <tr>
            <td><code>webdriver.Firefox().implicitly_wait()</code></td>
            <td>Instructs Selenium to wait a number of seconds, if it needs to. In the book, <code>webdriver.Firefox()</code> is assigned to a variable called <code>browser</code>, so that we can simply call <code>browser.implicitly_wait()</code>.</td>
        </tr>
        <tr>
            <td><code>webdriver.Firefox().quit()</code></td>
            <td>Close the currently-active browser. In the book, <code>webdriver.Firefox()</code> is assigned to a variable called <code>browser</code>, so that we can simply call <code>browser.quit()</code>.</td>
        </tr>
        <tr>
            <td><code>webdriver.Firefox().title</code></td>
            <td>Return the <code>&lt;title&gt;</code> of the active browser tab. In the book, <code>webdriver.Firefox()</code> is assigned to a variable called <code>browser</code>, so that we can simply call <code>browser.title</code>.</td>
        </tr>
    </tbody>
</table>

### Document Specific Commands

<em>Note, all of the following commands will assume you're prefixing them with a browser instance (for example <code>webdriver.Firefox()</code>).</em>

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>find_element_by_id()</code></td>
            <td>Returns a single document element by its ID.</td>
        </tr>
        <tr>
            <td><code>find_element_by_class_name()</code></td>
            <td>Returns a single document element by its CSS class.</td>
        </tr>
        <tr>
            <td><code>find_elements_by_class_name()</code></td>
            <td>Returns a list of document elements which match a given CSS class.</td>
        </tr>
        <tr>
            <td><code>find_element_by_tag_name()</code></td>
            <td>Returns a single document element by its HTML tag name.</td>
        </tr>
        <tr>
            <td><code>find_elements_by_tag_name()</code></td>
            <td>Returns a list of document elements which match a given HTML tag name.</td>
        </tr>
        <tr>
            <td><code>find_element_by_css_selector()</code></td>
            <td>Returns a single document element which matches a given CSS selector. Similar to how you target elements in CSS stylesheets.</td>
        </tr>
        <tr>
            <td><code>find_elements_by_css_selector()</code></td>
            <td>Returns a list of document elements which match a given CSS selector.</td>
        </tr>
    </tbody>
</table>

Additional selectors are outlined in the [Selenium Docs on Locating Elements](http://selenium-python.readthedocs.org/en/latest/locating-elements.html).
