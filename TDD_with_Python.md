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

## Django

### Core Commands

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>django-admin.py startproject name</code></td>
            <td>Starts a django project with a name of <code>name</code></td>
        </tr>
    </tbody>
</table>

### Test-Specific

<table>
    <thead>
        <tr>
            <th>Method</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code><em>SimpleTestCase</em>.assertTemplateUsed(response, template_name, msg_prefix='')</code></td>
            <td>Asserts that the template with the given name (string) was used in rendering the response.</td>
        </tr>
    </tbody>
</table>

## Python

### Test-Specific Methods

The following assertions come from the [Python 3 unittest Docs](https://docs.python.org/3/library/unittest)

<table>
<thead>
    <tr>
        <th>Method</th>
        <th>Checks that</th>
        <th>New in</th>
    </tr>
</thead>
<tbody>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertEqual" title="unittest.TestCase.assertEqual">assertEqual(a, b)</a></td>
        <td>a == b</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertNotEqual" title="unittest.TestCase.assertNotEqual">assertNotEqual(a, b)</a></td>
        <td>a != b</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertTrue" title="unittest.TestCase.assertTrue">assertTrue(x)</a></td>
        <td>bool(x) is True</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertFalse" title="unittest.TestCase.assertFalse">assertFalse(x)</a></td>
        <td>bool(x) is False</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIs" title="unittest.TestCase.assertIs">assertIs(a, b)</a></td>
        <td>a is b</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIsNot" title="unittest.TestCase.assertIsNot">assertIsNot(a, b)</a></td>
        <td>a is not b</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIsNone" title="unittest.TestCase.assertIsNone">assertIsNone(x)</a></td>
        <td>x is None</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIsNotNone" title="unittest.TestCase.assertIsNotNone">assertIsNotNone(x)</a></td>
        <td>x is not None</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIn" title="unittest.TestCase.assertIn">assertIn(a, b)</a></td>
        <td>a in b</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertNotIn" title="unittest.TestCase.assertNotIn">assertNotIn(a, b)</a></td>
        <td>a not in b</td>
        <td>3.1</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertIsInstance" title="unittest.TestCase.assertIsInstance">assertIsInstance(a, b)</a></td>
        <td>isinstance(a, b)</td>
        <td>3.2</td>
    </tr>
    <tr>
        <td><a href="https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertNotIsInstance" title="unittest.TestCase.assertNotIsInstance">assertNotIsInstance(a, b)</a></td>
        <td>not isinstance(a, b)</td>
        <td>3.2</td>
    </tr>
</tbody>
</table>

### Core Commands

<table>
    <thead>
        <tr>
            <th>Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>assert</code></td>
            <td>A statement with tests a condition. Example usage: <code>assert 'Django' in browser.title</code>. An additional expression can be added after a comma in the form of <code>assert expression1, expression2</code>. If <code>expression1</code> fails, <code>expression2</code> will be returned with the <code>AssertionError</code>.</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td><code>time.sleep(seconds)</code></td>
            <td>Useful for pausing a test during execution. Must be imported using <code>import time</code> Example usage: <code>time.sleep(3)</code>.</td>
        </tr>
    </tbody>
</table>