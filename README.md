# attendance-app
KONDLI BAZAR SECTOR-53 ONLY 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Attendance App</title>
<link rel="stylesheet" href="assets/style.css">
</head>
<body>
<div class="container">
  <div id="loginSection">
    <h2>Login</h2>
    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">
    <select id="role">
      <option value="">Select Role</option>
      <option value="admin">Admin</option>
      <option value="staff">Staff</option>
    </select>
    <button onclick="login()">Login</button>
    <p><a href="#" id="forgotPassword">Forgot Admin Password?</a></p>
  </div>

  <div id="adminDashboard" style="display:none;">
    <h2>Admin Panel</h2>
    <button onclick="logout()">Logout</button>
    <h3>Manage Staff</h3>
    <button onclick="addStaff()">Add Staff</button>
    <button onclick="editStaff()">Edit Staff</button>
    <h3>Attendance Reports</h3>
    <button onclick="exportAttendance()">📥 Export Attendance</button>
    <h3>Edit Profile</h3>
    <input type="text" id="newAdminName" placeholder="New Name">
    <input type="password" id="newAdminPass" placeholder="New Password">
    <button onclick="updateAdminProfile()">Update Profile</button>
  </div>

  <div id="staffDashboard" style="display:none;">
    <h2>Staff Panel</h2>
    <button onclick="logout()">Logout</button>
    <h3>Punch Attendance</h3>
    <input type="file" id="staffPhoto" accept="image/*">
    <button onclick="punchAttendance()">Punch Attendance</button>
    <div id="map"></div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/face-api.js"></script>
<script src="assets/app.js"></script>
</body>
</html>

