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
