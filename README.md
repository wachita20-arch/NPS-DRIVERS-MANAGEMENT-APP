<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>NPS TRANSPORT MANAGEMENT WEBSITE | National Police Standing Orders</title>
<meta name="description" content="NPS Transport Management Website - Standing Orders - Drivers Rank, Name, Age, Region, County/Formation, Station, Licence Validity, Classes, Vehicle Make & Number, Defects, Fuel Drawn Records">
<style>
*{box-sizing:border-box;margin:0;padding:0;font-family:Arial,sans-serif}
body{background:#eef1f5;color:#111}
a{color:inherit;text-decoration:none}
.topbar{background:#0b2c4a;color:#fff;padding:8px 20px;display:flex;justify-content:space-between;font-size:13px;flex-wrap:wrap;gap:8px}
.topbar b{color:#ffc107}
header{position:sticky;top:0;z-index:20;background:#fff;box-shadow:0 2px 10px rgba(0,0,0,.08)}
.nav{max-width:1280px;margin:auto;padding:14px 20px;display:flex;justify-content:space-between;align-items:center;gap:16px}
.logo{font-weight:900;font-size:22px;color:#0b2c4a;line-height:1}.logo span{font-size:11px;letter-spacing:1px;color:#1a7a3a}
.nav-links{display:flex;gap:18px;font-weight:700;font-size:14px}
.nav-links a:hover{color:#1a7a3a}
.btn{display:inline-block;padding:11px 18px;border-radius:10px;font-weight:800;border:0;cursor:pointer;text-align:center;font-size:14px}
.btn-green{background:#1a7a3a;color:#fff}.btn-dark{background:#0b2c4a;color:#fff}.btn-yellow{background:#ffc107;color:#000}.btn-wa{background:#25D366;color:#fff}.btn-red{background:#b71c1c;color:#fff}.btn-outline{background:#fff;border:2px solid #0b2c4a;color:#0b2c4a}
.wrap{max-width:1280px;margin:auto;padding:0 20px}
.hero{background:linear-gradient(135deg,#0b2c4a 0%,#123f6b 55%,#1a7a3a 100%);color:#fff;padding:28px 0}
.hero-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:24px;align-items:center}
.hero h1{font-size:38px;line-height:1.05}.hero h1 span{color:#ffc107}
.hero p{opacity:.92;margin:12px 0}
.pill{background:rgba(255,255,255,.15);border:1px solid rgba(255,255,255,.3);padding:6px 12px;border-radius:20px;font-size:13px;font-weight:700;display:inline-block}
section{padding:28px 0} h2{font-size:28px;color:#0b2c4a;margin-bottom:6px}.sub{color:#555;margin-bottom:16px}
.card{background:#fff;border-radius:14px;padding:18px;box-shadow:0 2px 12px rgba(0,0,0,.06);margin-bottom:16px}
.kpi{display:grid;grid-template-columns:repeat(6,1fr);gap:12px}
.kpi div{background:#fff;border-radius:12px;padding:14px;text-align:center;box-shadow:0 2px 10px rgba(0,0,0,.06)}
.kpi b{font-size:26px;color:#0b2c4a}.kpi span{font-size:12px;color:#555}
table{width:100%;border-collapse:collapse;font-size:13px;margin-top:10px}
th,td{border:1px solid #ddd;padding:9px;text-align:left;vertical-align:top}
th{background:#0b2c4a;color:#fff;position:sticky;top:0}
tr:nth-child(even){background:#f9f9f9}
input,select,textarea{width:100%;padding:11px;border:1px solid #ddd;border-radius:10px;margin:5px 0;font-size:15px}
label{font-size:13px;font-weight:700;color:#0b2c4a}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.grid3{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
.grid4{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}
.tabs{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:14px}
.tabs button{width:auto;padding:10px 16px;background:#eee;color:#222}
.tabs button.active{background:#0b2c4a;color:#fff}
.badge{display:inline-block;padding:4px 10px;border-radius:20px;font-size:11px;font-weight:800}
.alert-green{background:#e8f5e9;border:1px solid #1a7a3a;padding:12px;border-radius:10px;margin-bottom:12px}
.alert-orange{background:#fff3e0;border:2px solid #ef6c00;padding:12px;border-radius:10px;margin-bottom:12px;font-weight:700;color:#e65100}
.alert-red{background:#ffebee;border:2px solid #b71c1c;padding:12px;border-radius:10px;margin-bottom:12px;font-weight:700;color:#b71c1c}
.so-box{background:#fff3e0;border:2px solid #ef6c00;border-radius:12px;padding:14px}
.check label{display:block;background:#f6f6f6;padding:8px;border-radius:8px;margin:4px 0;font-size:13px}
.check input{width:auto;margin-right:8px}
.sidebar{position:fixed;left:0;top:0;bottom:0;width:250px;background:#0b2c4a;color:#fff;padding:20px;z-index:30;display:none}
.sidebar a{display:block;padding:11px;border-radius:8px;margin-bottom:6px;font-weight:700}
.sidebar a:hover,.sidebar a.active{background:#ffc107;color:#000}
.layout{display:grid;grid-template-columns:250px 1fr;gap:0}
.layout .side{position:sticky;top:70px;height:calc(100vh - 70px);background:#0b2c4a;color:#fff;padding:16px;overflow:auto}
.layout .side a{display:block;padding:11px;border-radius:8px;margin-bottom:6px;font-weight:700;color:#fff}
.layout .side a:hover,.layout .side a.active{background:#ffc107;color:#000}
.hidden{display:none}
@media(max-width:900px){.kpi{grid-template-columns:1fr 1fr 1fr}.grid2,.grid3,.grid4,.hero-grid{grid-template-columns:1fr}.layout{grid-template-columns:1fr}.layout .side{display:none}.nav-links{display:none}}
@media(max-width:560px){.kpi{grid-template-columns:1fr 1fr} table{font-size:12px} .hero h1{font-size:28px}}
.print-only{display:none}
@media print{body{background:#fff} header,.topbar,.tabs,.no-print,.hero,.sidebar,.layout .side{display:none!important} .print-only{display:block} .wrap{max-width:100%} .card{box-shadow:none;border:1px solid #ddd} }
</style>
</head>
<body>

<div class="topbar"><div>🇰🇪 REPUBLIC OF KENYA • <b>NATIONAL POLICE SERVICE</b> • MT BRANCH</div><div>📜 <b>STANDING ORDERS COMPLIANT</b> • 💬 <a href="https://wa.me/c/254777725770" target="_blank"><b>WhatsApp Channel →</b></a> • 📞 <b>0777 725 770</b></div></div>

<header><div class="nav">
  <div class="logo">🚔 NPS TRANSPORT<br><span>MANAGEMENT WEBSITE</span></div>
  <div class="nav-links"><a href="#dashboard">Dashboard</a><a href="#register">Drivers Register</a><a href="#vehicles">Vehicles</a><a href="#defects">Defects</a><a href="#fuel">Fuel Drawn</a><a href="#report">SO Report</a></div>
  <div style="display:flex;gap:8px"><button class="btn btn-wa" onclick="window.open('https://wa.me/c/254777725770','_blank')">💬 Channel</button><button class="btn btn-green" onclick="showSection('adddriver')">➕ Add Driver</button><button class="btn btn-dark" onclick="toggleLogin()">🔐 <span id="loginBtnText">Login: MT Officer</span></button></div>
</div></header>

<div class="hero"><div class="wrap hero-grid">
  <div>
    <span class="pill">📜 BASED ON NATIONAL POLICE STANDING ORDERS</span>
    <h1>TRANSPORT MANAGEMENT<br><span>STANDING ORDERS</span></h1>
    <p>Drivers Register • Vehicle Assignment • Defects • Fuel Drawn Records • Inspection • Daily Report. One Website for the whole Formation / Station / Region.</p>
    <div style="display:flex;gap:8px;flex-wrap:wrap"><span class="pill">✅ Licence Validity Check</span><span class="pill">✅ Classes Match Vehicle</span><span class="pill">✅ Defect Grounding</span><span class="pill">✅ Fuel Voucher Required</span></div>
    <div style="display:flex;gap:10px;margin-top:14px;flex-wrap:wrap"><button class="btn btn-yellow" onclick="showSection('register')">📜 View Drivers Register ↓</button><button class="btn btn-wa" onclick="window.open('https://wa.me/c/254777725770','_blank')">💬 WhatsApp Channel</button></div>
  </div>
  <div class="card" id="loginCard">
    <h3>🔐 Standing Orders Access</h3><p class="small" style="color:#555">Only authorised officers may access Transport Records.</p>
    <label>Officer Name *</label><input id="offName" placeholder="e.g. IP James Mwangi">
    <label>Service No. *</label><input id="offNo" placeholder="e.g. 567890" inputmode="numeric">
    <label>Role *</label><select id="offRole"><option>MT Officer - Transport Officer</option><option>OCS - Officer Commanding Station</option><option>Fleet Manager / Transport Manager</option><option>Inspector - Inspection Officer</option><option>Driver - View My Record Only</option></select>
    <label>Station / Formation</label><input id="offStation" placeholder="e.g. Eldoret Central - Rift Valley">
    <button class="btn btn-green" style="width:100%" onclick="doLogin()">Login →</button>
    <p class="small" style="color:#555;margin-top:8px">Demo: Any name + Service No. works. Driver role sees only own record.</p>
  </div>
</div></div>

<div class="layout">
  <div class="side no-print">
    <b style="color:#ffc107">📜 STANDING ORDERS MENU</b>
    <a href="#" id="side-dashboard" class="active" onclick="showSection('dashboard');return false">📊 Dashboard</a>
    <a href="#" id="side-register" onclick="showSection('register');return false">📜 Drivers Register (SO)</a>
    <a href="#" id="side-adddriver" onclick="showSection('adddriver');return false">➕ Add Driver (SO Form)</a>
    <a href="#" id="side-vehicles" onclick="showSection('vehicles');return false">🚔 Vehicles - Make & Number</a>
    <a href="#" id="side-assign" onclick="showSection('assign');return false">📋 Assign / Duty</a>
    <a href="#" id="side-defects" onclick="showSection('defects');return false">🔧 Defects</a>
    <a href="#" id="side-fuel" onclick="showSection('fuel');return false">⛽ Fuel Drawn Records</a>
    <a href="#" id="side-inspection" onclick="showSection('inspection');return false">✅ Daily Inspection (SO)</a>
    <a href="#" id="side-report" onclick="showSection('report');return false">📄 SO Report PDF</a>
    <hr style="margin:12px 0;border-color:rgba(255,255,255,.2)">
    <div style="font-size:12px;opacity:.9"><b>Logged in:</b> <span id="sideUser">Not logged in - Demo Mode</span><br><b>Station:</b> <span id="sideStation">Eldoret Central</span></div>
    <button class="btn btn-yellow" style="width:100%;margin-top:12px" onclick="printCurrent()">🖨️ Print Current Page</button>
    <button class="btn btn-wa" style="width:100%" onclick="window.open('https://wa.me/c/254777725770','_blank')">💬 WhatsApp Channel</button>
  </div>

  <div class="wrap" style="padding-top:18px">
    <div id="alertBox"></div>

    <!-- DASHBOARD -->
    <div id="dashboardSection">
      <h2>📊 Dashboard — Standing Orders Compliance</h2><p class="sub">Per Standing Orders, driver MUST have Valid Licence + Valid Classes for Vehicle + Vehicle Inspected + No Outstanding High Defect before assignment.</p>
      <div class="so-box"><b>📜 STANDING ORDERS COMPLIANCE</b><div style="display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin-top:10px"><div class="card" style="text-align:center;margin:0"><b id="soCompliant" style="font-size:28px;color:#1a7a3a">0</b><br><span class="small">✅ Compliant - Can Be Assigned</span></div><div class="card" style="text-align:center;margin:0"><b id="soNonCompliant" style="font-size:28px;color:#b71c1c">0</b><br><span class="small">⛔ Non-Compliant - Cannot Assign</span></div><div class="card" style="text-align:center;margin:0"><b id="soDefects" style="font-size:28px;color:#ef6c00">0</b><br><span class="small">🔧 Defects Open</span></div><div class="card" style="text-align:center;margin:0"><b id="soGrounded" style="font-size:28px;color:#b71c1c">0</b><br><span class="small">🚫 Vehicles Grounded</span></div></div></div>
      <div class="kpi" style="margin-top:12px">
        <div><b id="kDrivers">0</b><br><span>Drivers</span></div>
        <div><b id="kVehicles">0</b><br><span>Vehicles</span></div>
        <div><b id="kOnDuty" style="color:#1a7a3a">0</b><br><span>On Duty Today</span></div>
        <div><b id="kFuel" style="color:#ef6c00">Ksh 0</b><br><span>Fuel Drawn Today</span></div>
        <div><b id="kFuelLitres">0 L</b><br><span>Litres Today</span></div>
        <div><b id="kExpiring" style="color:#b71c1c">0</b><br><span>Licence Expiring &lt;30 Days</span></div>
      </div>
      <div class="grid2" style="margin-top:14px">
        <div class="card"><h3>⚠️ Urgent — Standing Orders</h3><div id="urgentList"></div></div>
        <div class="card"><h3>📋 Today's Assignments</h3><div id="todayAssignList"></div></div>
      </div>
    </div>

    <!-- REGISTER -->
    <div id="registerSection" class="hidden">
      <h2>📜 Drivers Register — Standing Orders Format</h2><p class="sub">Columns per Standing Orders: Rank | Name | Age | Region of Work | County / Formation of Work | Station | Licence Number | Validity | Driving Classes | Vehicle Make and Number Assigned</p>
      <div class="card">
        <div class="grid4">
          <div><label>Filter by Region</label><select id="drvRegionFilter" onchange="renderAll()"><option value="all">All Regions</option><option>Rift Valley</option><option>Nairobi</option><option>Central</option><option>Eastern</option><option>Western</option><option>Nyanza</option><option>Coast</option><option>North Eastern</option></select></div>
          <div><label>Filter by County / Formation</label><select id="drvCountyFilter" onchange="renderAll()"><option value="all">All Counties / Formations</option><option>Uasin Gishu</option><option>Trans Nzoia</option><option>Nairobi County</option><option>Kisumu</option><option>GSU Formation</option><option>AP Formation</option><option>Traffic Formation</option></select></div>
          <div><label>Filter by Status</label><select id="drvStatusFilter" onchange="renderAll()"><option value="all">All Status</option><option>Active</option><option>On Leave</option><option>Suspended</option><option>Off Duty</option></select></div>
          <div><label>Search</label><input id="drvSearch" placeholder="Rank, Name, Service No, Licence No, Vehicle No, Station..." oninput="renderAll()"></div>
        </div>
        <div style="display:flex;gap:8px;flex-wrap:wrap;margin-top:10px"><button class="btn btn-dark" onclick="printCurrent()">🖨️ Print Register</button><button class="btn btn-green" onclick="exportCSV()">📥 Export CSV</button><button class="btn btn-outline" onclick="showSection('adddriver')">➕ Add Driver</button></div>
        <div style="overflow-x:auto"><table><thead><tr><th>#</th><th>Rank</th><th>Name</th><th>Age</th><th>Region of Work</th><th>County / Formation</th><th>Station</th><th>Licence No.</th><th>Validity</th><th>Driving Classes</th><th>Vehicle Make & Number Assigned</th><th>SO Status</th><th class="no-print">Action</th></tr></thead><tbody id="registerBody"></tbody></table></div>
      </div>
    </div>

    <!-- ADD DRIVER -->
    <div id="adddriverSection" class="hidden">
      <h2>➕ Add Driver — Standing Orders Form</h2><p class="sub">All fields REQUIRED per Standing Orders. Driver cannot be assigned without complete record.</p>
      <div class="card">
        <div class="grid3">
          <div><label>1. RANK *</label><select id="dRank"><option>Constable - PC</option><option>Corporal - CPL</option><option>Sergeant - SGT</option><option>Senior Sergeant - SSGT</option><option>Inspector - IP</option><option>Chief Inspector - CIP</option><option>Superintendent - SP</option><option>Civilian Driver</option></select></div>
          <div><label>2. NAME *</label><input id="dName" placeholder="Full Name e.g. John Kamau"></div>
          <div><label>3. AGE *</label><input id="dAge" placeholder="Age e.g. 32" type="number" inputmode="numeric"></div>
          <div><label>4. SERVICE NO. *</label><input id="dService" placeholder="e.g. 123456" inputmode="numeric"></div>
          <div><label>5. ID NO.</label><input id="dId" placeholder="ID No." inputmode="numeric"></div>
          <div><label>6. PHONE</label><input id="dPhone" placeholder="Phone" inputmode="tel"></div>
          <div><label>7. REGION OF WORK *</label><select id="dRegion"><option>Rift Valley</option><option>Nairobi</option><option>Central</option><option>Eastern</option><option>Western</option><option>Nyanza</option><option>Coast</option><option>North Eastern</option></select></div>
          <div><label>8. COUNTY / FORMATION OF WORK *</label><select id="dCounty"><option>Uasin Gishu</option><option>Trans Nzoia</option><option>Elgeyo Marakwet</option><option>Nandi</option><option>Kericho</option><option>Bomet</option><option>Nakuru</option><option>Baringo</option><option>Turkana</option><option>West Pokot</option><option>Nairobi County</option><option>Kisumu</option><option>Mombasa</option><option>GSU Formation</option><option>AP Formation</option><option>Traffic Formation</option><option>Other Formation</option></select></div>
          <div><label>Formation (If Other)</label><input id="dFormationOther" placeholder="e.g. DCI, K9..."></div>
          <div><label>9. STATION *</label><input id="dStation" placeholder="e.g. Eldoret Central Police Station"></div>
          <div><label>10. LICENCE NUMBER *</label><input id="dLicenceNo" placeholder="e.g. DL123456"></div>
          <div><label>11. LICENCE VALIDITY * (Expiry)</label><input id="dLicenceExpiry" type="date"><div id="licenceCheck" class="small"></div></div>
        </div>
        <div style="margin-top:12px"><label>12. DRIVING CLASSES * (Tick all held)</label><div class="check" style="display:grid;grid-template-columns:repeat(3,1fr);gap:8px"><label><input type="checkbox" value="A" id="clsA"> Class A - Motorcycle</label><label><input type="checkbox" value="B" id="clsB" checked> Class B - Small Car / Probox</label><label><input type="checkbox" value="C" id="clsC"> Class C - Lorry</label><label><input type="checkbox" value="D" id="clsD"> Class D - Bus / PSV</label><label><input type="checkbox" value="BCE" id="clsBCE"> Class BCE - All Classes</label><label><input type="checkbox" value="E" id="clsE"> Class E - Trailer / Articulated</label></div></div>
        <div class="grid3" style="margin-top:12px">
          <div><label>13a. VEHICLE MAKE *</label><select id="dVehicleMake"><option>Toyota Land Cruiser</option><option>Toyota Hilux Double Cabin</option><option>Toyota Hiace Bus</option><option>Isuzu Lorry / Truck</option><option>Toyota Probox</option><option>Mitsubishi Outlander</option><option>Nissan Patrol</option><option>Motorcycle - Honda / Yamaha</option><option>Other Make</option></select></div>
          <div><label>13b. VEHICLE NUMBER ASSIGNED *</label><input id="dVehicleNo" placeholder="e.g. GKB 123A"></div>
          <div><label>14. EXPERIENCE (Years)</label><input id="dExperience" placeholder="e.g. 8" type="number" inputmode="numeric"></div>
          <div><label>TRAINING</label><select id="dTraining"><option>No Special Training</option><option>Defensive Driving - Ajira Driving School</option><option>Refresher - Ajira Driving School</option><option>VIP / Escort Driving</option><option>PSV Training</option><option>First Aid + Defensive</option></select></div>
          <div><label>STATUS</label><select id="dStatus"><option>Active</option><option>On Leave</option><option>Off Duty</option><option>Suspended</option></select></div>
          <div><label>NOTES (Discipline, Medical...)</label><input id="dNotes" placeholder="Standing Orders Notes..."></div>
        </div>
        <button class="btn btn-green" style="margin-top:12px" onclick="addDriver()">✅ Save Driver — Standing Orders Record</button>
      </div>
    </div>

    <!-- VEHICLES -->
    <div id="vehiclesSection" class="hidden">
      <h2>🚔 Vehicles — Vehicle Make and Number Assigned</h2>
      <div class="card"><h3>+ Add Vehicle</h3><div class="grid4"><div><label>Vehicle Make *</label><input id="vMake" placeholder="e.g. Toyota Land Cruiser"></div><div><label>Vehicle Number *</label><input id="vPlate" placeholder="e.g. GKB 123A"></div><div><label>Type</label><select id="vType"><option>Patrol Car</option><option>Double Cabin</option><option>Lorry / Truck</option><option>Bus</option><option>Motorcycle</option><option>Ambulance</option><option>Probox / Saloon</option></select></div><div><label>Mileage</label><input id="vMileage" placeholder="e.g. 125000" type="number" inputmode="numeric"></div><div><label>Fuel Type</label><select id="vFuelType"><option>Diesel</option><option>Petrol</option></select></div><div><label>Status</label><select id="vStatus"><option>Available - Fit for Duty</option><option>On Duty - Assigned</option><option>In Garage - Defect</option><option>Accident - Off Road</option><option>Grounded - Standing Orders</option></select></div><div><label>Chassis No.</label><input id="vChassis" placeholder="Chassis No."></div><div><label>&nbsp;</label><button class="btn btn-green" onclick="addVehicle()">Save Vehicle</button></div></div></div>
      <div class="card"><div style="overflow-x:auto"><table><thead><tr><th>Vehicle Make</th><th>Vehicle Number</th><th>Type</th><th>Chassis</th><th>Mileage</th><th>Fuel</th><th>Status</th><th>Driver Assigned</th><th>Open Defects</th><th>Fuel Drawn Total</th></tr></thead><tbody id="vehicleBody"></tbody></table></div></div>
    </div>

    <!-- ASSIGN -->
    <div id="assignSection" class="hidden">
      <h2>📋 Assign Driver — Standing Orders Check</h2><p class="sub">App BLOCKS assignment if: Licence Expired OR Classes do NOT match Vehicle OR Vehicle has Open High Defect OR Driver Suspended.</p>
      <div class="card">
        <div class="grid2">
          <div><label>Driver (Rank + Name + Service No.)</label><select id="aDriver" onchange="updateAssignCheck()"></select><div id="aDriverInfo" class="small"></div></div>
          <div><label>Vehicle Make & Number</label><select id="aVehicle" onchange="updateAssignCheck()"></select><div id="soAssignCheck" class="small"></div></div>
          <div><label>Date</label><input id="aDate" type="date"></div>
          <div><label>Time</label><input id="aTime" type="time"></div>
          <div><label>Duty</label><select id="aDuty"><option>Patrol - Town Patrol</option><option>Patrol - Highway Patrol</option><option>Escort - VIP / Cash Escort</option><option>Response - Emergency Response</option><option>Transport - Prisoners / Staff</option><option>Training - Ajira Driving School</option><option>Standby - Station Standby</option></select></div>
          <div><label>Area</label><input id="aLocation" placeholder="e.g. Eldoret Town - CBD"></div>
          <div><label>Purpose</label><input id="aPurpose" placeholder="e.g. Night Patrol CBD to Langas"></div>
          <div><label>&nbsp;</label><button class="btn btn-green" style="width:100%" onclick="assignDriver()">📋 Assign — Pass Standing Orders Check</button></div>
        </div>
      </div>
      <div class="card"><h3>Assignments List</h3><div style="overflow-x:auto"><table><thead><tr><th>Date / Time</th><th>Rank + Name</th><th>Vehicle Make & Number</th><th>Duty</th><th>Area / Purpose</th><th>SO Check</th><th>Status</th><th class="no-print">Action</th></tr></thead><tbody id="assignBody"></tbody></table></div></div>
    </div>

    <!-- DEFECTS -->
    <div id="defectsSection" class="hidden">
      <h2>🔧 Defects — Standing Orders</h2><p class="sub">Per Standing Orders, driver MUST report any defect BEFORE and AFTER duty. Vehicle with High Defect CANNOT be assigned.</p>
      <div class="card"><div class="grid3"><div><label>Vehicle Make & Number</label><select id="mVehicle"></select></div><div><label>Driver Reporting</label><select id="mDriver"></select></div><div><label>Defect Type</label><select id="mType"><option>Defect - Brakes</option><option>Defect - Tyres / Puncture</option><option>Defect - Engine</option><option>Defect - Lights / Electrical</option><option>Defect - Steering</option><option>Defect - Accident Damage</option><option>Defect - Body / Windscreen</option><option>Service - Routine Service Due</option><option>Other Defect</option></select></div><div><label>Description *</label><input id="mDesc" placeholder="Describe defect in detail..."></div><div><label>Priority</label><select id="mPriority"><option>Low - Can Wait - Vehicle Can Still Move</option><option>Medium - Fix This Week - Monitor</option><option>High - GROUND VEHICLE - Do NOT Assign (Standing Orders)</option></select></div><div><label>Estimated Cost Ksh</label><input id="mCost" placeholder="Cost Ksh" type="number" inputmode="numeric"></div></div><button class="btn btn-red" style="margin-top:10px" onclick="reportDefect()">🔧 Report Defect</button></div>
      <div class="card"><label>Filter Defects</label><select id="defectFilter" onchange="renderAll()"><option value="all">All Defects</option><option value="Pending">Pending / Open</option><option value="Fixed">Fixed / Closed</option><option value="High">High - Grounded Only</option></select><div style="overflow-x:auto"><table><thead><tr><th>Date</th><th>Vehicle Make & Number</th><th>Driver</th><th>Defect Type</th><th>Description</th><th>Priority</th><th>Cost</th><th>Status</th><th class="no-print">Action</th></tr></thead><tbody id="defectBody"></tbody></table></div></div>
    </div>

    <!-- FUEL -->
    <div id="fuelSection" class="hidden">
      <h2>⛽ Fuel Drawn Records — Standing Orders</h2><p class="sub">Per Standing Orders, every fuel drawn MUST be recorded: Vehicle, Driver, Litres, Amount, KM, Voucher, Station. No fuel without voucher.</p>
      <div class="card"><div class="grid3"><div><label>Vehicle Make & Number</label><select id="fVehicle"></select></div><div><label>Driver (Rank + Name)</label><select id="fDriver"></select></div><div><label>Litres Drawn *</label><input id="fLitres" placeholder="e.g. 40" type="number" inputmode="numeric"></div><div><label>Amount Ksh *</label><input id="fAmount" placeholder="e.g. 8000" type="number" inputmode="numeric"></div><div><label>KM Reading at Fuel *</label><input id="fKm" placeholder="e.g. 125000" type="number" inputmode="numeric"></div><div><label>Fuel Voucher / Receipt No. *</label><input id="fVoucher" placeholder="e.g. VCH001"></div><div><label>Fuel Station</label><select id="fStation"><option>Shell - Eldoret</option><option>TotalEnergies - Eldoret</option><option>Rubis - Kitale</option><option>NPS Fuel Depot - Eldoret</option><option>NPS Fuel Depot - Kitale</option><option>Other Station</option></select></div><div><label>Purpose</label><select id="fPurpose"><option>Patrol Duty</option><option>Escort Duty</option><option>Emergency Response</option><option>Transport Duty</option><option>Training</option></select></div><div><label>&nbsp;</label><button class="btn btn-green" style="width:100%" onclick="saveFuel()">⛽ Save Fuel Drawn Record</button></div></div></div>
      <div class="card" style="background:#e3f2fd"><b>⛽ Fuel Summary</b><div id="fuelSummary" class="small"></div></div>
      <div class="card"><label>Filter Fuel</label><select id="fuelFilter" onchange="renderAll()"><option value="all">All Fuel</option><option value="today">Today Only</option><option value="month">This Month</option></select><div style="overflow-x:auto"><table><thead><tr><th>Date</th><th>Vehicle Make & Number</th><th>Driver (Rank + Name)</th><th>Litres</th><th>Amount Ksh</th><th>KM</th><th>Voucher No.</th><th>Station</th><th>Purpose</th><th>Officer</th></tr></thead><tbody id="fuelBody"></tbody></table></div></div>
    </div>

    <!-- INSPECTION -->
    <div id="inspectionSection" class="hidden">
      <h2>✅ Daily Vehicle Inspection — Standing Orders</h2><p class="sub">Driver MUST inspect vehicle before duty. Tick ALL. If any FAIL, report defect and DO NOT move vehicle.</p>
      <div class="card"><div class="grid2"><div><label>Vehicle Make & Number</label><select id="iVehicle"></select></div><div><label>Driver Inspecting</label><select id="iDriver"></select></div></div>
        <div class="check" style="display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-top:10px"><label><input type="checkbox" id="chkBrakes" checked> Brakes - Working</label><label><input type="checkbox" id="chkTyres" checked> Tyres - Pressure + Condition</label><label><input type="checkbox" id="chkLights" checked> Lights - Headlights, Indicators</label><label><input type="checkbox" id="chkOil" checked> Oil + Water + Coolant</label><label><input type="checkbox" id="chkSteering" checked> Steering - Working</label><label><input type="checkbox" id="chkMirrors" checked> Mirrors + Windscreen + Wipers</label><label><input type="checkbox" id="chkFuel" checked> Fuel - Enough for Duty</label><label><input type="checkbox" id="chkDocs" checked> Documents - Log Book, Insurance, Licence</label><label><input type="checkbox" id="chkFirstAid" checked> First Aid + Fire Extinguisher + Spare Tyre + Jack</label></div>
        <label style="margin-top:10px">Inspection Notes</label><input id="iNotes" placeholder="Inspection notes..."><button class="btn btn-green" style="margin-top:10px" onclick="saveInspection()">✅ Save Inspection — Pass / Fail</button>
      </div>
      <div class="card"><div style="overflow-x:auto"><table><thead><tr><th>Date</th><th>Vehicle Make & Number</th><th>Driver</th><th>Result</th><th>Checks</th><th>Notes</th></tr></thead><tbody id="inspectionBody"></tbody></table></div></div>
    </div>

    <!-- REPORT -->
    <div id="reportSection" class="hidden">
      <h2>📄 Standing Orders Transport Report</h2>
      <div class="card"><div class="grid3"><div><label>Month</label><input type="month" id="reportMonth"></div><div><label>&nbsp;</label><button class="btn btn-green" style="width:100%" onclick="generateReport()">Generate SO Report PDF</button></div><div><label>&nbsp;</label><button class="btn btn-wa" style="width:100%" onclick="shareReport()">Share via WhatsApp</button></div></div></div>
      <div id="reportPreview"></div>
    </div>

    <footer style="padding:20px 0;text-align:center;color:#555;font-size:13px">🇰🇪 NATIONAL POLICE SERVICE • MT BRANCH • STANDING ORDERS<br>Learn • Serve • Protect • Drive Safe • 💬 <a href="https://wa.me/c/254777725770" target="_blank" style="color:#25D366;font-weight:900">WhatsApp Channel →</a> • 📞 0777 725 770<br>© 2026 NPS Transport Management Website — Based on National Police Standing Orders</footer>
  </div>
</div>

<script>
let LANG = "en";
let drivers = JSON.parse(localStorage.getItem("nps_web_drivers")||"[]");
let vehicles = JSON.parse(localStorage.getItem("nps_web_vehicles")||"[]");
let assignments = JSON.parse(localStorage.getItem("nps_web_assignments")||"[]");
let defects = JSON.parse(localStorage.getItem("nps_web_defects")||"[]");
let fuels = JSON.parse(localStorage.getItem("nps_web_fuel")||"[]");
let inspections = JSON.parse(localStorage.getItem("nps_web_inspections")||"[]");
let currentUser={name:"Demo - MT Officer",role:"MT Officer - Transport Officer",station:"Eldoret Central - Rift Valley"};
let isOfficer=true;
function getToday(){ return new Date().toISOString().slice(0,10); }
function getCurrentMonth(){ return new Date().toISOString().slice(0,7); }
function daysToExpiry(d){ if(!d) return 999; return Math.ceil((new Date(d)-new Date())/(1000*60*60*24)); }
function isCompliant(d){ return daysToExpiry(d.licenceExpiry)>=0 && d.status!=="Suspended" && !defects.find(x=>x.vehicleNo===d.vehicleNo && x.priority.includes("High") && x.status.includes("Pending")); }
function vehicleNeedsClass(make){ if(make.includes("Lorry")||make.includes("Truck")) return ["C","BCE","E"]; if(make.includes("Bus")) return ["D","BCE"]; if(make.includes("Motorcycle")) return ["A","BCE"]; return ["B","BCE","C","D","E"]; }
function toggleLogin(){ document.getElementById("loginCard").scrollIntoView({behavior:"smooth"}); }
function doLogin(){ let n=document.getElementById("offName").value.trim(); let no=document.getElementById("offNo").value.trim(); let role=document.getElementById("offRole").value; let st=document.getElementById("offStation").value.trim(); if(!n||!no) return alert("Enter Officer Name and Service No."); currentUser={name:n,no,role,station:st||"Eldoret Central"}; isOfficer=!role.includes("Driver"); document.getElementById("loginBtnText").innerText="Logged: "+n; document.getElementById("sideUser").innerText=n+" ("+role+")"; document.getElementById("sideStation").innerText=st||"Eldoret Central"; alert("✅ Logged in: "+n+" - "+role); renderAll(); }
function showSection(sec){
  ["dashboard","register","adddriver","vehicles","assign","defects","fuel","inspection","report"].forEach(k=>{ let el=document.getElementById(k+"Section"); if(el) el.classList.toggle("hidden",k!==sec); });
  document.querySelectorAll(".side a").forEach(a=>a.classList.remove("active"));
  let side=document.getElementById("side-"+sec); if(side) side.classList.add("active");
  renderAll(); window.scrollTo({top:0,behavior:"smooth"});
}
function printCurrent(){ window.print(); }
function exportCSV(){
  let header="Rank,Name,Age,Region,County/Formation,Station,Licence No,Validity,Classes,Vehicle Make,Vehicle Number,Status\n";
  let rows=drivers.map(d=>`"${d.rank}","${d.name}",${d.age},"${d.region}","${d.county} ${d.formation}","${d.station}","${d.licenceNo}",${d.licenceExpiry},"${d.classes.join(" ")}","${d.vehicleMake}","${d.vehicleNo}","${d.status}"`).join("\n");
  let blob=new Blob([header+rows],{type:"text/csv"}); let a=document.createElement("a"); a.href=URL.createObjectURL(blob); a.download="NPS_Drivers_Register_"+getToday()+".csv"; a.click();
}
function addDriver(){
  let rank=document.getElementById("dRank").value; let name=document.getElementById("dName").value.trim(); let age=parseInt(document.getElementById("dAge").value||0); let svc=document.getElementById("dService").value.trim(); let idNo=document.getElementById("dId").value.trim(); let phone=document.getElementById("dPhone").value.trim(); let region=document.getElementById("dRegion").value; let county=document.getElementById("dCounty").value; let formationOther=document.getElementById("dFormationOther").value.trim(); let station=document.getElementById("dStation").value.trim(); let licNo=document.getElementById("dLicenceNo").value.trim(); let licExp=document.getElementById("dLicenceExpiry").value; let vehicleMake=document.getElementById("dVehicleMake").value; let vehicleNo=document.getElementById("dVehicleNo").value.trim(); let exp=document.getElementById("dExperience").value; let training=document.getElementById("dTraining").value; let status=document.getElementById("dStatus").value; let notes=document.getElementById("dNotes").value.trim();
  let classes=[]; ["A","B","C","D","BCE","E"].forEach(c=>{ if(document.getElementById("cls"+c)?.checked) classes.push(c); });
  if(!name||!svc||!age||!station||!licNo||!licExp||!vehicleNo) return alert("Fill ALL Standing Orders fields: Rank, Name, Age, Service No, Station, Licence No, Validity, Vehicle No.");
  if(classes.length===0) return alert("Tick at least ONE Driving Class");
  if(drivers.find(d=>d.serviceNo===svc)) return alert("Service No. already exists!");
  drivers.unshift({id:Date.now(),rank,name,age,serviceNo:svc,idNo,phone,region,county,formation:formationOther,station,licenceNo:licNo,licenceExpiry:licExp,classes,vehicleMake,vehicleNo,experience:exp,training,status,notes,createdAt:new Date().toISOString(),day:getToday()}); localStorage.setItem("nps_web_drivers",JSON.stringify(drivers));
  ["dName","dAge","dService","dId","dPhone","dStation","dLicenceNo","dVehicleNo","dExperience","dNotes","dFormationOther"].forEach(id=>document.getElementById(id).value="");
  alert("✅ STANDING ORDERS RECORD SAVED\n"+rank+" "+name+" - "+svc+"\nAge: "+age+" • Region: "+region+" • County/Formation: "+county+" "+formationOther+"\nStation: "+station+"\nLicence: "+licNo+" - Valid to "+licExp+"\nClasses: "+classes.join(", ")+"\nVehicle: "+vehicleMake+" - "+vehicleNo);
  showSection('register');
}
function addVehicle(){
  let make=document.getElementById("vMake").value.trim(); let plate=document.getElementById("vPlate").value.trim(); let type=document.getElementById("vType").value; let chassis=document.getElementById("vChassis").value.trim(); let mileage=document.getElementById("vMileage").value; let fuelType=document.getElementById("vFuelType").value; let status=document.getElementById("vStatus").value;
  if(!make||!plate) return alert("Enter Vehicle Make and Number");
  vehicles.unshift({id:Date.now(),make,plate,type,chassis,mileage:parseInt(mileage||0),fuelType,status,driver:"-"}); localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles));
  ["vMake","vPlate","vChassis","vMileage"].forEach(id=>document.getElementById(id).value="");
  alert("Vehicle Added: "+make+" - "+plate); renderAll();
}
function updateAssignCheck(){
  let driverId=document.getElementById("aDriver").value; let vehicleVal=document.getElementById("aVehicle").value; let drv=drivers.find(d=>d.id==driverId); if(!drv) return;
  document.getElementById("aDriverInfo").innerHTML="<b>"+drv.rank+" "+drv.name+" - "+drv.serviceNo+"</b><br>Age: "+drv.age+" • Region: "+drv.region+" • County/Formation: "+drv.county+" "+drv.formation+"<br>Station: "+drv.station+"<br>Licence: "+drv.licenceNo+" - Valid to "+drv.licenceExpiry+" ("+daysToExpiry(drv.licenceExpiry)+" days)<br>Classes: "+drv.classes.join(", ")+" • Assigned Vehicle: "+drv.vehicleMake+" - "+drv.vehicleNo;
  let veh=vehicles.find(v=>v.plate===vehicleVal.split(" - ")[0]); if(!veh) return;
  let needed=vehicleNeedsClass(veh.make); let hasClass=drv.classes.some(c=>needed.includes(c)||c==="BCE");
  let highDefect=defects.find(x=>x.vehicleNo===veh.plate && x.priority.includes("High") && x.status.includes("Pending"));
  let licExpired=daysToExpiry(drv.licenceExpiry)<0; let suspended=drv.status==="Suspended";
  let checks=[]; checks.push(licExpired?"⛔ LICENCE EXPIRED":"✅ Licence Valid"); checks.push(hasClass?"✅ Classes Match Vehicle ("+needed.join("/")+" - Driver has "+drv.classes.join(", ")+")":"⛔ CLASSES DO NOT MATCH - Vehicle needs "+needed.join("/")+" - Driver has "+drv.classes.join(", ")); checks.push(highDefect?"⛔ HIGH DEFECT OPEN - GROUNDED - "+highDefect.type:"✅ No High Defect"); checks.push(suspended?"⛔ DRIVER SUSPENDED":"✅ Driver Active");
  let pass=!licExpired && hasClass && !highDefect && !suspended;
  document.getElementById("soAssignCheck").innerHTML="<div style='background:"+(pass?"#e8f5e9":"#ffebee")+";border:2px solid "+(pass?"#1a7a3a":"#b71c1c")+";border-radius:8px;padding:10px;margin-top:8px'><b>"+(pass?"✅ STANDING ORDERS: PASS - CAN ASSIGN":"⛔ STANDING ORDERS: FAIL - CANNOT ASSIGN")+"</b><br>"+checks.join("<br>")+"</div>";
}
function assignDriver(){
  let driverId=document.getElementById("aDriver").value; let vehicleVal=document.getElementById("aVehicle").value; let date=document.getElementById("aDate").value; let time=document.getElementById("aTime").value; let duty=document.getElementById("aDuty").value; let loc=document.getElementById("aLocation").value.trim(); let purpose=document.getElementById("aPurpose").value.trim();
  if(!driverId||!date) return alert("Select Driver and Date");
  let drv=drivers.find(d=>d.id==driverId); let veh=vehicles.find(v=>v.plate===vehicleVal.split(" - ")[0]);
  let needed=vehicleNeedsClass(veh.make); let hasClass=drv.classes.some(c=>needed.includes(c)||c==="BCE");
  let highDefect=defects.find(x=>x.vehicleNo===veh.plate && x.priority.includes("High") && x.status.includes("Pending"));
  if(daysToExpiry(drv.licenceExpiry)<0) return alert("⛔ STANDING ORDERS BLOCKED: "+drv.name+" LICENCE EXPIRED on "+drv.licenceExpiry+". Cannot assign until renewed.");
  if(!hasClass) return alert("⛔ STANDING ORDERS BLOCKED: "+drv.name+" Classes "+drv.classes.join(", ")+" do NOT match "+veh.make+" which needs "+needed.join("/")+ ".\nSend driver to Ajira Driving School to add Class.");
  if(highDefect) return alert("⛔ STANDING ORDERS BLOCKED: Vehicle "+veh.plate+" has HIGH DEFECT: "+highDefect.type+" - "+highDefect.desc+". Fix defect first.");
  if(drv.status==="Suspended") return alert("⛔ STANDING ORDERS BLOCKED: "+drv.name+" is Suspended.");
  let clash=assignments.find(a=>a.driverId==drv.id && a.date===date && a.status.includes("Active"));
  if(clash) return alert(drv.name+" already assigned on "+date+" - "+clash.duty);
  assignments.unshift({id:Date.now(),driverId:drv.id,name:drv.name,rank:drv.rank,vehicleMake:veh.make,vehicleNo:veh.plate,date,time,duty,location:loc,purpose,status:"Active - On Duty",officer:currentUser.name,soCheck:"PASSED - Licence Valid, Classes Match, No High Defect"}); localStorage.setItem("nps_web_assignments",JSON.stringify(assignments));
  drv.vehicleMake=veh.make; drv.vehicleNo=veh.plate; drv.status="Active"; localStorage.setItem("nps_web_drivers",JSON.stringify(drivers));
  veh.status="On Duty - Assigned"; veh.driver=drv.rank+" "+drv.name; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles));
  alert("✅ STANDING ORDERS PASSED - ASSIGNED!\n"+drv.rank+" "+drv.name+" - "+drv.serviceNo+"\nVehicle: "+veh.make+" - "+veh.plate+"\nDuty: "+duty+"\nDate: "+date+" "+time+"\nArea: "+loc);
  renderAll();
}
function completeAssignment(id){ let a=assignments.find(x=>x.id===id); if(!a) return; a.status="Completed - Back at Station"; localStorage.setItem("nps_web_assignments",JSON.stringify(assignments)); renderAll(); }
function reportDefect(){
  let vehicleVal=document.getElementById("mVehicle").value; let driverName=document.getElementById("mDriver").value; let type=document.getElementById("mType").value; let desc=document.getElementById("mDesc").value.trim(); let priority=document.getElementById("mPriority").value; let cost=parseInt(document.getElementById("mCost").value||0);
  if(!vehicleVal||!desc) return alert("Select Vehicle and Describe Defect");
  let veh=vehicles.find(v=>v.plate===vehicleVal.split(" - ")[0]);
  defects.unshift({id:Date.now(),vehicleMake:veh.make,vehicleNo:veh.plate,driver:driverName,type,desc,priority,cost,status:"Pending - Waiting for Parts",date:getToday(),officer:currentUser.name}); localStorage.setItem("nps_web_defects",JSON.stringify(defects));
  if(priority.includes("High")){ veh.status="In Garage - Defect"; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles)); }
  alert("Defect Reported: "+veh.make+" - "+veh.plate+" - "+type+" - "+priority); document.getElementById("mDesc").value=""; renderAll();
}
function fixDefect(id){ let d=defects.find(x=>x.id===id); if(!d) return; d.status="Fixed - Vehicle Back on Road"; localStorage.setItem("nps_web_defects",JSON.stringify(defects)); let veh=vehicles.find(v=>v.plate===d.vehicleNo); if(veh && veh.status.includes("Garage")){ veh.status="Available - Fit for Duty"; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles)); } alert("Fixed: "+d.vehicleMake+" - "+d.vehicleNo+" - "+d.type); renderAll(); }
function saveFuel(){
  let vehicleVal=document.getElementById("fVehicle").value; let driverVal=document.getElementById("fDriver").value; let litres=parseFloat(document.getElementById("fLitres").value||0); let amount=parseInt(document.getElementById("fAmount").value||0); let km=parseInt(document.getElementById("fKm").value||0); let voucher=document.getElementById("fVoucher").value.trim(); let station=document.getElementById("fStation").value; let purpose=document.getElementById("fPurpose").value;
  if(!vehicleVal||!litres||!amount||!voucher) return alert("Fill Vehicle, Litres, Amount AND Voucher No. - Standing Orders: No fuel without voucher.");
  let veh=vehicles.find(v=>v.plate===vehicleVal.split(" - ")[0]);
  fuels.unshift({id:Date.now(),vehicleMake:veh.make,vehicleNo:veh.plate,driver:driverVal,litres,amount,km,voucher,station,purpose,date:getToday(),officer:currentUser.name}); localStorage.setItem("nps_web_fuel",JSON.stringify(fuels));
  veh.mileage=km; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles));
  alert("Fuel Drawn Record Saved: "+veh.make+" - "+veh.plate+" - "+litres+" L - Ksh "+amount.toLocaleString()+" - Voucher "+voucher);
  ["fLitres","fAmount","fKm","fVoucher"].forEach(id=>document.getElementById(id).value=""); renderAll();
}
function saveInspection(){
  let vehicleVal=document.getElementById("iVehicle").value; let driverVal=document.getElementById("iDriver").value; let notes=document.getElementById("iNotes").value.trim();
  let checks={brakes:document.getElementById("chkBrakes").checked,tyres:document.getElementById("chkTyres").checked,lights:document.getElementById("chkLights").checked,oil:document.getElementById("chkOil").checked,steering:document.getElementById("chkSteering").checked,mirrors:document.getElementById("chkMirrors").checked,fuel:document.getElementById("chkFuel").checked,docs:document.getElementById("chkDocs").checked,firstAid:document.getElementById("chkFirstAid").checked};
  let failed=Object.keys(checks).filter(k=>!checks[k]);
  let veh=vehicles.find(v=>v.plate===vehicleVal.split(" - ")[0]);
  let result=failed.length===0?"PASS - Fit for Duty":"FAIL - DO NOT MOVE - Failed: "+failed.join(", ");
  inspections.unshift({id:Date.now(),vehicleMake:veh.make,vehicleNo:veh.plate,driver:driverVal,result,checks:failed.length?"Failed: "+failed.join(", "):"All 9 Checks Passed",notes,date:getToday(),officer:currentUser.name}); localStorage.setItem("nps_web_inspections",JSON.stringify(inspections));
  if(failed.length>0){ defects.unshift({id:Date.now()+1,vehicleMake:veh.make,vehicleNo:veh.plate,driver:driverVal,type:"Defect - Inspection Failed",desc:"Inspection FAILED: "+failed.join(", ")+" - "+notes,priority:"High - GROUND VEHICLE - Do NOT Assign (Standing Orders)",cost:0,status:"Pending - Waiting for Parts",date:getToday(),officer:currentUser.name}); localStorage.setItem("nps_web_defects",JSON.stringify(defects)); veh.status="In Garage - Defect"; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles)); }
  alert("Inspection: "+veh.make+" - "+veh.plate+"\n"+result); renderAll();
}
function generateReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let mFuel=fuels.filter(x=>x.date && x.date.startsWith(month)); let mDefects=defects.filter(x=>x.date && x.date.startsWith(month)); let html="<div id='soReportPrint' style='background:#fff;border:1px solid #ddd;padding:18px'><div style='text-align:center'><div>🇰🇪 REPUBLIC OF KENYA</div><h2>NATIONAL POLICE SERVICE</h2><div>TRANSPORT MANAGEMENT REPORT - STANDING ORDERS</div><div>Month: "+month+" • Station: Eldoret Central • Region: Rift Valley</div><hr></div><p>Drivers: "+drivers.length+" • Compliant: "+drivers.filter(d=>isCompliant(d)).length+" • Non-Compliant: "+drivers.filter(d=>!isCompliant(d)).length+"<br>Vehicles: "+vehicles.length+" • Assignments: "+assignments.length+"<br>Fuel Drawn This Month: "+mFuel.reduce((sum,x)=>sum+x.litres,0)+" L • Ksh "+mFuel.reduce((sum,x)=>sum+x.amount,0).toLocaleString()+"<br>Defects This Month: "+mDefects.length+" • Open: "+defects.filter(x=>x.status.includes("Pending")).length+"</p><h4>1. DRIVERS REGISTER - STANDING ORDERS</h4><table><tr><th>Rank</th><th>Name</th><th>Age</th><th>Region</th><th>County/Formation</th><th>Station</th><th>Licence No.</th><th>Validity</th><th>Classes</th><th>Vehicle Make & No.</th></tr>"+drivers.map(d=>"<tr><td>"+d.rank+"</td><td>"+d.name+"</td><td>"+d.age+"</td><td>"+d.region+"</td><td>"+d.county+" "+d.formation+"</td><td>"+d.station+"</td><td>"+d.licenceNo+"</td><td>"+d.licenceExpiry+" ("+daysToExpiry(d.licenceExpiry)+" days)</td><td>"+d.classes.join(", ")+"</td><td>"+d.vehicleMake+" - "+d.vehicleNo+"</td></tr>").join("")+"</table><h4>2. DEFECTS</h4>"+defects.map(x=>"<div>"+x.date+" - "+x.vehicleMake+" "+x.vehicleNo+" - "+x.type+" - "+x.desc+" - "+x.priority+" - "+x.status+"</div>").join("")+"<h4>3. FUEL DRAWN RECORDS</h4><table><tr><th>Date</th><th>Vehicle</th><th>Driver</th><th>Litres</th><th>Amount</th><th>KM</th><th>Voucher</th><th>Station</th></tr>"+mFuel.map(x=>"<tr><td>"+x.date+"</td><td>"+x.vehicleMake+" "+x.vehicleNo+"</td><td>"+x.driver+"</td><td>"+x.litres+" L</td><td>Ksh "+x.amount.toLocaleString()+"</td><td>"+x.km+"</td><td>"+x.voucher+"</td><td>"+x.station+"</td></tr>").join("")+"</table><br><br><table style='border:0'><tr><td style='border:0'>MT Officer:<br><br>______________<br>"+currentUser.name+"</td><td style='border:0;text-align:right'>OCS / Stamp:<br><br>______________</td></tr></table></div><button class='btn btn-green' onclick='window.print()'>🖨️ Print / Save PDF</button>"; document.getElementById("reportPreview").innerHTML=html; }
function shareReport(){ let month=document.getElementById("reportMonth").value||getCurrentMonth(); let txt="🇰🇪 NPS TRANSPORT REPORT - STANDING ORDERS\nMonth: "+month+"\nDrivers: "+drivers.length+" • Compliant: "+drivers.filter(d=>isCompliant(d)).length+" • Non-Compliant: "+drivers.filter(d=>!isCompliant(d)).length+"\nVehicles: "+vehicles.length+" • Fuel: "+fuels.reduce((sum,x)=>sum+x.litres,0)+" L - Ksh "+fuels.reduce((sum,x)=>sum+x.amount,0).toLocaleString()+"\nDefects Open: "+defects.filter(x=>x.status.includes("Pending")).length; window.open("https://wa.me/?text="+encodeURIComponent(txt),"_blank"); }

function initData(){
  if(drivers.length===0){
    drivers=[
      {id:1,rank:"Constable - PC",name:"John Kamau",age:32,serviceNo:"123456",idNo:"30111111",phone:"0711111111",region:"Rift Valley",county:"Uasin Gishu",formation:"",station:"Eldoret Central Police Station",licenceNo:"DL111222",licenceExpiry:"2027-03-15",classes:["B","C"],vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 123A",experience:8,training:"Defensive Driving - Ajira Driving School",status:"Active",notes:"No discipline case"},
      {id:2,rank:"Sergeant - SGT",name:"Mary Wanjiru",age:38,serviceNo:"234567",idNo:"30222222",phone:"0722222222",region:"Rift Valley",county:"Uasin Gishu",formation:"",station:"Eldoret Central Police Station",licenceNo:"DL333444",licenceExpiry:"2026-12-10",classes:["B","D"],vehicleMake:"Toyota Hiace Bus",vehicleNo:"GKB 101D",experience:12,training:"PSV Training",status:"Active",notes:"First Aid trained"},
      {id:3,rank:"Corporal - CPL",name:"Peter Otieno",age:29,serviceNo:"345678",idNo:"30333333",phone:"0733333333",region:"Rift Valley",county:"Trans Nzoia",formation:"",station:"Kitale Police Station",licenceNo:"DL555666",licenceExpiry:"2026-11-30",classes:["C"],vehicleMake:"Isuzu Lorry / Truck",vehicleNo:"GKB 789C",experience:6,training:"No Special Training",status:"On Leave",notes:"On leave until 30 Nov"},
      {id:4,rank:"Constable - PC",name:"David Kiprop",age:26,serviceNo:"456789",idNo:"30444444",phone:"0744444444",region:"Rift Valley",county:"Uasin Gishu",formation:"Traffic Formation",station:"Eldoret Central Police Station",licenceNo:"DL777888",licenceExpiry:"2027-06-20",classes:["B"],vehicleMake:"Toyota Hilux Double Cabin",vehicleNo:"GKB 456B",experience:3,training:"Needs Defensive - Ajira Driving School",status:"Active",notes:"New driver"},
      {id:5,rank:"Inspector - IP",name:"James Mwangi",age:45,serviceNo:"567890",idNo:"30555555",phone:"0755555555",region:"Nairobi",county:"Nairobi County",formation:"GSU Formation",station:"GSU Headquarters - Nairobi",licenceNo:"DL999000",licenceExpiry:"2027-01-15",classes:["B","C","D","BCE"],vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 999Z",experience:18,training:"VIP / Escort Driving",status:"Active",notes:"GSU - VIP Escort"},
      {id:6,rank:"Sergeant - SGT",name:"Grace Chebet",age:35,serviceNo:"678901",idNo:"30666666",phone:"0766666666",region:"Rift Valley",county:"Nandi",formation:"",station:"Kapsabet Police Station",licenceNo:"DL111999",licenceExpiry:"2026-11-25",classes:["B","C"],vehicleMake:"Toyota Probox",vehicleNo:"GKB 222K",experience:9,training:"Defensive Driving - Ajira",status:"Active",notes:""},
    ]; localStorage.setItem("nps_web_drivers",JSON.stringify(drivers));
    vehicles=[
      {id:1,make:"Toyota Land Cruiser",plate:"GKB 123A",type:"Patrol Car",chassis:"JT123456",mileage:125000,fuelType:"Diesel",status:"On Duty - Assigned",driver:"PC John Kamau"},
      {id:2,make:"Toyota Hilux Double Cabin",plate:"GKB 456B",type:"Double Cabin",chassis:"JT456789",mileage:98000,fuelType:"Diesel",status:"On Duty - Assigned",driver:"PC David Kiprop"},
      {id:3,make:"Isuzu Lorry / Truck",plate:"GKB 789C",type:"Lorry / Truck",chassis:"IS789012",mileage:210000,fuelType:"Diesel",status:"In Garage - Defect",driver:"-"},
      {id:4,make:"Toyota Hiace Bus",plate:"GKB 101D",type:"Bus",chassis:"TH101234",mileage:156000,fuelType:"Diesel",status:"Available - Fit for Duty",driver:"SGT Mary Wanjiru"},
      {id:5,make:"Toyota Land Cruiser",plate:"GKB 999Z",type:"Patrol Car",chassis:"JT999000",mileage:85000,fuelType:"Diesel",status:"Available - Fit for Duty",driver:"IP James Mwangi"},
      {id:6,make:"Toyota Probox",plate:"GKB 222K",type:"Probox / Saloon",chassis:"TP222000",mileage:112000,fuelType:"Petrol",status:"Available - Fit for Duty",driver:"SGT Grace Chebet"},
    ]; localStorage.setItem("nps_web_vehicles",JSON.stringify(vehicles));
    assignments=[
      {id:1,driverId:1,name:"John Kamau",rank:"Constable - PC",vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 123A",date:getToday(),time:"08:00",duty:"Patrol - Town Patrol",location:"Eldoret Town - CBD",purpose:"Day Patrol CBD to Langas",status:"Active - On Duty",officer:"MT Officer",soCheck:"PASSED - Licence Valid, Classes B+C Match Land Cruiser, No Defect"},
      {id:2,driverId:4,name:"David Kiprop",rank:"Constable - PC",vehicleMake:"Toyota Hilux Double Cabin",vehicleNo:"GKB 456B",date:getToday(),time:"09:00",duty:"Escort - VIP / Cash Escort",location:"Eldoret - Kitale Road",purpose:"Cash Escort to Kitale",status:"Active - On Duty",officer:"MT Officer",soCheck:"PASSED - Licence Valid, Class B Match Double Cabin"},
      {id:3,driverId:2,name:"Mary Wanjiru",rank:"Sergeant - SGT",vehicleMake:"Toyota Hiace Bus",vehicleNo:"GKB 101D",date:getToday(),time:"10:00",duty:"Transport - Prisoners / Staff",location:"Eldoret - Eldoret Law Courts",purpose:"Prisoners to Court",status:"Active - On Duty",officer:"MT Officer",soCheck:"PASSED - Licence Valid, Class D Match Bus"},
    ]; localStorage.setItem("nps_web_assignments",JSON.stringify(assignments));
    defects=[
      {id:1,vehicleMake:"Isuzu Lorry / Truck",vehicleNo:"GKB 789C",driver:"CPL Peter Otieno",type:"Defect - Brakes",desc:"Brakes are soft, need check - DO NOT DRIVE",priority:"High - GROUND VEHICLE - Do NOT Assign (Standing Orders)",cost:15000,status:"Pending - Waiting for Parts",date:getToday(),officer:"MT Officer"},
      {id:2,vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 123A",driver:"PC John Kamau",type:"Service - Routine Service Due",desc:"10,000km service due next week",priority:"Medium - Fix This Week - Monitor",cost:12000,status:"Scheduled",date:getToday(),officer:"MT Officer"},
    ]; localStorage.setItem("nps_web_defects",JSON.stringify(defects));
    fuels=[
      {id:1,vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 123A",driver:"PC John Kamau",litres:40,amount:8000,km:125000,voucher:"VCH001",station:"Shell - Eldoret",purpose:"Patrol Duty",date:getToday(),officer:"MT Officer"},
      {id:2,vehicleMake:"Toyota Hilux Double Cabin",vehicleNo:"GKB 456B",driver:"PC David Kiprop",litres:35,amount:7000,km:98000,voucher:"VCH002",station:"NPS Fuel Depot - Eldoret",purpose:"Escort Duty",date:getToday(),officer:"MT Officer"},
      {id:3,vehicleMake:"Toyota Hiace Bus",vehicleNo:"GKB 101D",driver:"SGT Mary Wanjiru",litres:50,amount:10000,km:156000,voucher:"VCH003",station:"TotalEnergies - Eldoret",purpose:"Transport Duty",date:"2026-11-22",officer:"MT Officer"},
      {id:4,vehicleMake:"Toyota Probox",vehicleNo:"GKB 222K",driver:"SGT Grace Chebet",litres:25,amount:5000,km:112000,voucher:"VCH004",station:"Shell - Kapsabet",purpose:"Patrol Duty",date:getToday(),officer:"MT Officer"},
    ]; localStorage.setItem("nps_web_fuel",JSON.stringify(fuels));
    inspections=[{id:1,vehicleMake:"Toyota Land Cruiser",vehicleNo:"GKB 123A",driver:"PC John Kamau",result:"PASS - Fit for Duty",checks:"All 9 Checks Passed",notes:"All OK",date:getToday(),officer:"MT Officer"}];
    localStorage.setItem("nps_web_inspections",JSON.stringify(inspections));
  }
}
function renderAll(){
  initData();
  if(document.getElementById("reportMonth") && !document.getElementById("reportMonth").value) document.getElementById("reportMonth").value=getCurrentMonth();
  if(!document.getElementById("aDate").value) document.getElementById("aDate").value=getToday();
  // Dropdowns
  document.getElementById("aDriver").innerHTML=drivers.map(d=>"<option value='"+d.id+"'>"+d.rank+" "+d.name+" - "+d.serviceNo+" - "+d.licenceNo+" - Classes "+d.classes.join(", ")+" - "+d.status+"</option>").join("");
  document.getElementById("aVehicle").innerHTML=vehicles.map(v=>"<option value='"+v.plate+" - "+v.make+"'>"+v.make+" - "+v.plate+" - "+v.status+"</option>").join("");
  document.getElementById("mVehicle").innerHTML=vehicles.map(v=>"<option value='"+v.plate+" - "+v.make+"'>"+v.make+" - "+v.plate+"</option>").join("");
  document.getElementById("mDriver").innerHTML=drivers.map(d=>"<option value='"+d.rank+" "+d.name+"'>"+d.rank+" "+d.name+" - "+d.serviceNo+"</option>").join("");
  document.getElementById("fVehicle").innerHTML=vehicles.map(v=>"<option value='"+v.plate+" - "+v.make+"'>"+v.make+" - "+v.plate+"</option>").join("");
  document.getElementById("fDriver").innerHTML=drivers.map(d=>"<option value='"+d.rank+" "+d.name+"'>"+d.rank+" "+d.name+" - "+d.serviceNo+" - "+d.licenceNo+"</option>").join("");
  document.getElementById("iVehicle").innerHTML=vehicles.map(v=>"<option value='"+v.plate+" - "+v.make+"'>"+v.make+" - "+v.plate+"</option>").join("");
  document.getElementById("iDriver").innerHTML=drivers.map(d=>"<option value='"+d.rank+" "+d.name+"'>"+d.rank+" "+d.name+" - "+d.serviceNo+"</option>").join("");
  if(document.getElementById("dLicenceExpiry").value){ let days=daysToExpiry(document.getElementById("dLicenceExpiry").value); document.getElementById("licenceCheck").innerHTML=days<0?"<b style='color:#b71c1c'>⛔ EXPIRED "+Math.abs(days)+" days ago</b>":days<30?"<b style='color:#ef6c00'>⚠️ Expires in "+days+" days - Renew soon</b>":"<b style='color:#1a7a3a'>✅ Valid - "+days+" days left</b>"; }
  updateAssignCheck();
  // KPIs
  document.getElementById("kDrivers").innerText=drivers.length;
  document.getElementById("kVehicles").innerText=vehicles.length;
  document.getElementById("kOnDuty").innerText=assignments.filter(a=>a.date===getToday() && a.status.includes("Active")).length;
  document.getElementById("kFuel").innerText="Ksh "+fuels.filter(x=>x.date===getToday()).reduce((sum,x)=>sum+x.amount,0).toLocaleString();
  document.getElementById("kFuelLitres").innerText=fuels.filter(x=>x.date===getToday()).reduce((sum,x)=>sum+x.litres,0)+" L";
  document.getElementById("kExpiring").innerText=drivers.filter(d=>daysToExpiry(d.licenceExpiry)<30).length;
  document.getElementById("soCompliant").innerText=drivers.filter(d=>isCompliant(d)).length;
  document.getElementById("soNonCompliant").innerText=drivers.filter(d=>!isCompliant(d)).length;
  document.getElementById("soDefects").innerText=defects.filter(x=>x.status.includes("Pending")).length;
  document.getElementById("soGrounded").innerText=vehicles.filter(v=>v.status.includes("Garage")||v.status.includes("Grounded")).length;
  // Alerts
  let alertHtml="";
  let expiring=drivers.filter(d=>daysToExpiry(d.licenceExpiry)<30);
  if(expiring.length) alertHtml+="<div class='alert-red'>⚠️ LICENCE EXPIRING: "+expiring.map(d=>d.rank+" "+d.name+" - "+d.licenceNo+" - "+d.licenceExpiry+" ("+daysToExpiry(d.licenceExpiry)+" days)").join(" • ")+"</div>";
  let highDef=defects.filter(x=>x.priority.includes("High") && x.status.includes("Pending"));
  if(highDef.length) alertHtml+="<div class='alert-red'>🔧 HIGH DEFECT - GROUNDED: "+highDef.map(x=>x.vehicleMake+" "+x.vehicleNo+" - "+x.type).join(" • ")+"</div>";
  if(!alertHtml) alertHtml="<div class='alert-green'>✅ All drivers compliant with Standing Orders. All vehicles fit for duty.</div>";
  document.getElementById("alertBox").innerHTML=alertHtml;
  document.getElementById("urgentList").innerHTML=(expiring.length?expiring.map(d=>"<div style='padding:8px;border-bottom:1px solid #eee'>⚠️ <b>"+d.rank+" "+d.name+"</b> — Licence "+d.licenceNo+" expires "+d.licenceExpiry+" ("+daysToExpiry(d.licenceExpiry)+" days) — <b>Renew Now</b></div>").join(""):"")+(highDef.length?highDef.map(x=>"<div style='padding:8px;border-bottom:1px solid #eee'>🔧 <b>"+x.vehicleMake+" "+x.vehicleNo+"</b> — "+x.type+" — "+x.desc+" — <b>GROUNDED</b></div>").join(""):"")+(!expiring.length && !highDef.length?"<p class='small'>No urgent items.</p>":"");
  document.getElementById("todayAssignList").innerHTML=assignments.filter(a=>a.date===getToday()).length?assignments.filter(a=>a.date===getToday()).map(a=>"<div style='padding:8px;border-bottom:1px solid #eee'><b>"+a.rank+" "+a.name+"</b> — "+a.vehicleMake+" "+a.vehicleNo+" — "+a.duty+" — "+a.time+" — "+a.location+"</div>").join(""):"<p class='small'>No assignments today.</p>";
  // Register Table
  let rf=document.getElementById("drvRegionFilter")?.value||"all"; let cf=document.getElementById("drvCountyFilter")?.value||"all"; let sf=document.getElementById("drvStatusFilter")?.value||"all"; let ss=document.getElementById("drvSearch")?.value.toLowerCase()||"";
  let fDrivers=drivers.filter(d=>{ if(rf!=="all" && d.region!==rf) return false; if(cf!=="all" && !(d.county===cf || (d.formation && d.formation.includes(cf)))) return false; if(sf!=="all" && d.status!==sf) return false; return (d.rank+" "+d.name+" "+d.serviceNo+" "+d.licenceNo+" "+d.vehicleNo+" "+d.station+" "+d.county+" "+d.region).toLowerCase().includes(ss); });
  document.getElementById("registerBody").innerHTML=fDrivers.length?fDrivers.map((d,i)=>{ let days=daysToExpiry(d.licenceExpiry); let licColor=days<0?"#b71c1c":days<30?"#ef6c00":"#1a7a3a"; let comp=isCompliant(d); return "<tr><td>"+(i+1)+"</td><td><b>"+d.rank+"</b></td><td><b>"+d.name+"</b><br><span class='small'>Service: "+d.serviceNo+" • ID: "+d.idNo+" • "+d.phone+"</span></td><td>"+d.age+"</td><td>"+d.region+"</td><td>"+d.county+"<br><span class='small'>"+(d.formation||"")+"</span></td><td>"+d.station+"</td><td><b>"+d.licenceNo+"</b></td><td><b style='color:"+licColor+"'>"+d.licenceExpiry+"<br>("+days+" days)</b></td><td><b>"+d.classes.join(", ")+"</b></td><td><b>"+d.vehicleMake+"</b><br><b>"+d.vehicleNo+"</b></td><td><span class='badge' style='background:"+(comp?"#1a7a3a":"#b71c1c")+";color:#fff'>"+(comp?"✅ COMPLIANT":"⛔ NON-COMPLIANT")+"</span><br><span class='small'>"+d.status+"</span></td><td class='no-print'><button class='btn btn-outline' style='padding:6px 10px;font-size:12px' onclick=\"alert('Driver: "+d.rank+" "+d.name+"\\nService: "+d.serviceNo+"\\nTraining: "+d.training+"\\nNotes: "+d.notes+"')\">View</button></td></tr>"; }).join(""):"<tr><td colspan='13'>No drivers found.</td></tr>";
  // Vehicles
  document.getElementById("vehicleBody").innerHTML=vehicles.map(v=>{ let vDefects=defects.filter(x=>x.vehicleNo===v.plate && x.status.includes("Pending")); let vFuel=fuels.filter(x=>x.vehicleNo===v.plate); return "<tr><td><b>"+v.make+"</b></td><td><b>"+v.plate+"</b></td><td>"+v.type+"</td><td>"+v.chassis+"</td><td>"+v.mileage.toLocaleString()+" KM</td><td>"+v.fuelType+"</td><td><span class='badge' style='background:"+(v.status.includes("Available")?"#1a7a3a":v.status.includes("Garage")||v.status.includes("Grounded")?"#b71c1c":"#ef6c00")+";color:#fff'>"+v.status+"</span></td><td>"+v.driver+"</td><td><b style='color:"+(vDefects.length?"#b71c1c":"#1a7a3a")+"'>"+vDefects.length+"</b></td><td>"+vFuel.reduce((sum,x)=>sum+x.litres,0)+" L - Ksh "+vFuel.reduce((sum,x)=>sum+x.amount,0).toLocaleString()+"</td></tr>"; }).join("");
  // Assignments
  document.getElementById("assignBody").innerHTML=assignments.length?assignments.map(a=>"<tr><td>"+a.date+"<br>"+a.time+"</td><td><b>"+a.rank+" "+a.name+"</b></td><td><b>"+a.vehicleMake+"</b><br>"+a.vehicleNo+"</td><td>"+a.duty+"</td><td>"+a.location+"<br><span class='small'>"+a.purpose+"</span></td><td><span class='small'>"+(a.soCheck||"-")+"</span></td><td><span class='badge'>"+a.status+"</span></td><td class='no-print'>"+(a.status.includes("Active")?"<button class='btn btn-green' style='padding:6px 10px;font-size:12px' onclick='completeAssignment("+a.id+")'>✅ Complete</button>":"-")+"</td></tr>").join(""):"<tr><td colspan='8'>No assignments.</td></tr>";
  // Defects
  let df=document.getElementById("defectFilter")?.value||"all";
  let fDefects=defects.filter(x=>{ if(df==="Pending" && !x.status.includes("Pending")) return false; if(df==="Fixed" && !x.status.includes("Fixed")) return false; if(df==="High" && !x.priority.includes("High")) return false; return true; });
  document.getElementById("defectBody").innerHTML=fDefects.length?fDefects.map(x=>"<tr><td>"+x.date+"</td><td><b>"+x.vehicleMake+"</b><br>"+x.vehicleNo+"</td><td>"+x.driver+"</td><td>"+x.type+"</td><td>"+x.desc+"</td><td><b style='color:"+(x.priority.includes("High")?"#b71c1c":x.priority.includes("Medium")?"#ef6c00":"#1a7a3a")+"'>"+x.priority+"</b></td><td>Ksh "+x.cost.toLocaleString()+"</td><td>"+x.status+"</td><td class='no-print'>"+(x.status.includes("Pending")?"<button class='btn btn-green' style='padding:6px 10px;font-size:12px' onclick='fixDefect("+x.id+")'>🔧 Fix</button>":"✅")+"</td></tr>").join(""):"<tr><td colspan='9'>No defects.</td></tr>";
  // Fuel
  let ff=document.getElementById("fuelFilter")?.value||"all";
  let fFuel=fuels.filter(x=>{ if(ff==="today" && x.date!==getToday()) return false; if(ff==="month" && !x.date.startsWith(getCurrentMonth())) return false; return true; });
  let fuelLitresTotal=fFuel.reduce((sum,x)=>sum+x.litres,0); let fuelAmtTotal=fFuel.reduce((sum,x)=>sum+x.amount,0);
  document.getElementById("fuelSummary").innerHTML="Records: "+fFuel.length+" • Total Litres: <b>"+fuelLitresTotal+" L</b> • Total Amount: <b>Ksh "+fuelAmtTotal.toLocaleString()+"</b> • Avg Price: Ksh "+(fuelLitresTotal?(fuelAmtTotal/fuelLitresTotal).toFixed(0):0)+" / L";
  document.getElementById("fuelBody").innerHTML=fFuel.length?fFuel.map(x=>"<tr><td>"+x.date+"</td><td><b>"+x.vehicleMake+"</b><br>"+x.vehicleNo+"</td><td>"+x.driver+"</td><td><b>"+x.litres+" L</b></td><td><b>Ksh "+x.amount.toLocaleString()+"</b></td><td>"+x.km.toLocaleString()+" KM</td><td><b>"+x.voucher+"</b></td><td>"+x.station+"</td><td>"+x.purpose+"</td><td>"+x.officer+"</td></tr>").join(""):"<tr><td colspan='10'>No fuel records.</td></tr>";
  // Inspections
  document.getElementById("inspectionBody").innerHTML=inspections.length?inspections.map(x=>"<tr><td>"+x.date+"</td><td><b>"+x.vehicleMake+"</b><br>"+x.vehicleNo+"</td><td>"+x.driver+"</td><td><span class='badge' style='background:"+(x.result.includes("PASS")?"#1a7a3a":"#b71c1c")+";color:#fff'>"+x.result+"</span></td><td>"+x.checks+"</td><td>"+(x.notes||"")+"</td></tr>").join(""):"<tr><td colspan='6'>No inspections.</td></tr>";
}
renderAll();
</script>
</body>
</html>
