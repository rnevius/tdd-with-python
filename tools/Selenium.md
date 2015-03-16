## Selenium

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
            <td>Imports access to the <a href="http://docs.seleniumhq.org/docs/03_webdriver.jsp#introducing-webdriver">Selenium Webdriver API</a>.</td>
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
            <td><code>find_element_by_id()</code></td>
            <td>Returns a list of document elements which match a given ID.</td>
        </tr>
        <tr>
            <td><code>find_element_by_tag_name()</code></td>
            <td>Returns a single document element by its HTML tag name.</td>
        </tr>
        <tr>
            <td><code>find_elements_by_tag_name()</code></td>
            <td>Returns a list of document elements which match a given HTML tag name.</td>
        </tr>
    </tbody>
</table>