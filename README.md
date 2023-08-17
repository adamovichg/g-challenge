<!DOCTYPE html>
<html lang="en">

<h1>Bonus Calculator challenge</h1>
<h2>Objective: Prepare a New Bonus Calculator Tool</h2>
<p>The goal is to develop a Bonus Calculator, an integral tool designed to guide online casino players in selecting the most advantageous bonus according to specific conditions or requirements.</p>
<hr>

<h3>Resources:</h3>
<ol>
    <li><strong>Design and Instructions:</strong> An in-depth layout, visualization, and instructions for this task can be found on <a href="https://www.figma.com/file/LJ03WKi5RjP40BlqP8NcKn/Task?type=design&node-id=0%3A1&mode=design&t=wFlzcBIjNnM05URD-1">Figma</a>.</li>
    <li><strong>Bonus Data:</strong> This is stored in the table <code>g_bonuses</code>. The requisite script to create and populate this table is attached.</li>
</ol>

<h3>Column Descriptions for <code>g_bonuses</code> Table:</h3>
<table>
    <tr>
        <th>Column Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>id</td>
        <td>Unique identifier for the bonus</td>
    </tr>
    <tr>
        <td>casino_id</td>
        <td>Casino unique identifier</td>
    </tr>
    <tr>
        <td>type</td>
        <td>Bonus type</td>
    </tr>
    <tr>
        <td>crypto_short_description</td>
        <td>Short description (for crypto deposits)</td>
    </tr>
    <tr>
        <td>wagering</td>
        <td>Wagering requirement (how many times the bonus money should be wagered to fulfill requirements)</td>
    </tr>
    <tr>
        <td>code</td>
        <td>Bonus code</td>
    </tr>
    <tr>
        <td>recalculated_wagering_on_bonus</td>
        <td>Not all wagering is calculated the same, so this is a unified parameter</td>
    </tr>
    <tr>
        <td>min_deposit_usd</td>
        <td>Minimum deposit needed to get the bonus</td>
    </tr>
</table>
    <h3>Your tasks:</h3>
    <ol>
        <li>Set up your WordPress development environment with Docker and Docker Compose, import the <code>g_bonuses</code> table into the database, and populate it using the provided SQL script.</li>
        <li>Design a WordPress (or pure PHP) form according to the sections illustrated in the Figma file.</li>
        <li>Create a WordPress web-service (in the form of a WordPress plugin) that returns bonus data in JSON format to be shown in the results section of the PHP form.</li>
        <li>Develop and integrate a JavaScript function that gets triggered when the "Calculate" button is clicked. This should invoke the WordPress web service from the previous step and showcase the results in the aforementioned form.</li>
    </ol>
<p>
    <h3>Helpful Hints:</h3>
    <ol>
        <li>Utilize your Linux machine or opt for WSL if on Windows.</li>
        <li>Ensure Docker and Docker Compose are installed.</li>
        <li>Build or rebuild Docker services using the command: <code>docker compose build</code>.</li>
        <li>Start the services with the command: <code>docker compose up</code>.</li>
        <li>The service should be accessible on port 80 (or another designated port like 8080 as defined in <code>docker-compose.yml</code>). Verify by accessing localhost in your browser.</li>
        <li>Employ DBeaver for database connectivity and ensure you've opened the necessary ports and granted permissions for external user connections.</li>
    </ol>

<p>By following these instructions, you can help us prepare the new Bonus Calculator tool tailored to the needs of online casino players
