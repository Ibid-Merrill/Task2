# Task2
To-Do List Web App
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>To-Do List App</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <div class="app">
    <h1>My To-Do List</h1>
    <div class="input-group">
      <input type="text" id="task-input" placeholder="Enter a new task..." />
      <button id="add-button">Add</button>
    </div>
    <ul id="task-list"></ul>
  </div>

  <script src="script.js"></script>
</body>
</html>

/* Reset & Base Styles */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  display: flex;
  justify-content: center;
  padding: 50px;
}

.app {
  background: white;
  padding: 30px;
  width: 100%;
  max-width: 400px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

h1 {
  text-align: center;
  margin-bottom: 20px;
}

.input-group {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
}

#task-input {
  flex: 1;
  padding: 10px;
  font-size: 16px;
}

#add-button {
  padding: 10px 15px;
  background-color: #28a745;
  color: white;
  border: none;
  cursor: pointer;
  font-weight: bold;
  border-radius: 4px;
}

#add-button:hover {
  background-color: #218838;
}

#task-list {
  list-style: none;
}

.task {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #e9ecef;
  padding: 10px;
  margin-bottom: 10px;
  border-left: 5px solid #007bff;
  transition: background-color 0.3s;
}

.task.completed {
  text-decoration: line-through;
  background-color: #d4edda;
  color: #6c757d;
  border-left: 5px solid #28a745;
}

.task span {
  cursor: pointer;
  flex-grow: 1;
}

.task button {
  background-color: #dc3545;
  color: white;
  border: none;
  padding: 6px 10px;
  cursor: pointer;
  border-radius: 4px;
  font-size: 14px;
}

.task button:hover {
  background-color: #c82333;
}
