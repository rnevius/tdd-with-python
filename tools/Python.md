## Python

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
