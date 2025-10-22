<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Team Registration Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f5f5f5;
      margin: 40px;
    }
    form {
      background-color: white;
      padding: 20px;
      border-radius: 10px;
      max-width: 600px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin-top: 10px;
      font-weight: bold;
    }
    input, select, textarea, button {
      width: 100%;
      margin-top: 5px;
      padding: 8px;
      border-radius: 5px;
      border: 1px solid #ccc;
      box-sizing: border-box;
    }
    fieldset {
      margin-top: 15px;
      border: 1px solid #ccc;
      padding: 10px;
      border-radius: 8px;
    }
    legend {
      font-weight: bold;
    }
    .checkbox-group, .radio-group {
      display: flex;
      flex-direction: column;
      gap: 5px;
      margin-top: 5px;
    }
    button {
      background-color: #007bff;
      color: white;
      border: none;
      cursor: pointer;
      font-size: 16px;
      margin-top: 15px;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>

  <h1>Team Registration Form</h1>

  <form action="#" method="post">
    <!-- Team Name -->
    <label for="teamName">Team Name:</label>
    <input type="text" id="teamName" name="teamName" required>

    <!-- Team Principal -->
    <label for="teamPrincipal">Team Principal:</label>
    <input type="text" id="teamPrincipal" name="teamPrincipal" required>

    <!-- Contact Email -->
    <label for="contactEmail">Contact Email:</label>
    <input type="email" id="contactEmail" name="contactEmail" required>

    <!-- Car Number -->
    <label for="carNumber">Car Number (1–99):</label>
    <input type="number" id="carNumber" name="carNumber" min="1" max="99" required>

    <!-- Founding Year -->
    <label for="foundingYear">Founding Year:</label>
    <input type="date" id="foundingYear" name="foundingYear" required>

    <!-- Engine Supplier -->
    <fieldset>
      <legend>Engine Supplier</legend>
      <div class="radio-group">
        <label><input type="radio" name="engineSupplier" value="Mercedes" required> Mercedes</label>
        <label><input type="radio" name="engineSupplier" value="Honda"> Honda</label>
        <label><input type="radio" name="engineSupplier" value="Ferrari"> Ferrari</label>
        <label><input type="radio" name="engineSupplier" value="Renault"> Renault</label>
      </div>
    </fieldset>

    <!-- Technical Focus Areas -->
    <fieldset>
      <legend>Technical Focus Areas</legend>
      <div class="checkbox-group">
        <label><input type="checkbox" name="focusAreas" value="Aerodynamics"> Aerodynamics</label>
        <label><input type="checkbox" name="focusAreas" value="Powertrain"> Powertrain</label>
        <label><input type="checkbox" name="focusAreas" value="Chassis"> Chassis</label>
        <label><input type="checkbox" name="focusAreas" value="Pit Strategy"> Pit Strategy</label>
      </div>
    </fieldset>

    <!-- Home Circuit -->
    <label for="homeCircuit">Home Circuit:</label>
    <select id="homeCircuit" name="homeCircuit" required>
      <option value="">-- Select a Circuit --</option>
      <option value="Silverstone">Silverstone</option>
      <option value="Monaco">Monaco</option>
      <option value="Spa-Francorchamps">Spa-Francorchamps</option>
      <option value="Monza">Monza</option>
      <option value="Suzuka">Suzuka</option>
    </select>

    <!-- Team Biography -->
    <label for="biography">Team Biography:</label>
    <textarea id="biography" name="biography" rows="5" placeholder="Write about your team's history and goals..." required></textarea>

    <!-- Agreement -->
    <label>
      <input type="checkbox" id="agreement" name="agreement" required>
      I agree to the FIA Code of Conduct
    </label>

    <!-- Submit Button -->
    <button type="submit">Register for Championship</button>
  </form>

</body>
</html>

