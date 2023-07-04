<h1>Week #13 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>1. Age Prediction API 👶-👴</h2>

~~~javascript
const express = require("express");
const app = express();
const port = 3000;

app.get("/api/age/:name", (req, res) => {
  const name = req.params.name;

  if (!name) {
    return res
      .status(400)
      .json({ error: "Missing parameter 'name' was expected." });
  }

  const age = Math.floor(Math.random() * 100);
  const days = age * 365;

  const response = {
    name: name,
    age: age.toString(),
    days: days.toString(),
  };

  res.json(response);
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});

~~~
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/afae53aa-b893-4b1d-9f69-2c2a08d114ac">
<h2>2. NSA Secrets Box API - Hacking Challenge 👨‍💻</h2>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/a0cd0437-92a4-4b94-aff7-be2964089f9e">

<h2>3. The SQL Murder Mystery Walkthrough - Learning Exercise</h2>
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/9fd61edb-ef97-4014-9d8f-7e6f13b7ae29">
