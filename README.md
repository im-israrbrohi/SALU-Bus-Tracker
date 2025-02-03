# SALU Bus Tracker - Project Documentation

## 1. Project Overview
SALU Bus Tracker is an Android application designed for Shah Abdul Latif University to track university buses in real-time. The app serves three types of users: Students, Drivers, and Administrators.

## 2. Core Components

### 2.1 Authentication System
- **Files:**
  - `LoginActivity.kt`: Handles user login
  - `RegisterActivity.kt`: New user registration
  - `RequestAccessActivity.kt`: Request access to the system
  - `RequestAccountActivity.kt`: Request new account creation

### 2.2 User Dashboards

#### 1. Student Dashboard (`StudentDashboardActivity.kt`)
- View real-time bus locations
- Send messages to drivers
- View bus routes and schedules
- Submit complaints

#### 2. Driver Dashboard (`DriverDashboardActivity.kt`)
- Share real-time location
- View total distance traveled
- Receive student messages
- Set bus status (Active/Inactive)

#### 3. Admin Dashboard (`AdminActivity.kt`)
- Manage user accounts
- View system reports
- Handle access requests
- Monitor bus operations

### 2.3 Map System (`MapActivity.kt`)
- Real-time bus tracking using OpenStreetMap
- Custom markers for buses
- Location updates
- Route visualization

### 2.4 Communication System
- **`MessagesActivity.kt`**: Message handling
- **`NotifyStudentsActivity.kt`**: Send notifications to students
- **`RequestDriverActivity.kt`**: Student-driver communication

### 2.5 Support System
- **`ComplainActivity.kt`**: Handle student complaints
- **`BugReportActivity.kt`**: System issue reporting
- **`AboutProjectActivity.kt`**: Project information

## 3. Resources and Configuration

### 3.1 Layout Files (in `res/layout/`)

#### 1. Activity Layouts:
- `activity_login.xml`: Login screen
- `activity_register.xml`: Registration form
- `activity_student_dashboard.xml`: Student main screen
- `activity_driver_dashboard.xml`: Driver main screen
- `activity_map.xml`: Map view
- `activity_messages.xml`: Messaging interface
- `activity_notify_students.xml`: Student notification screen

#### 2. Custom Layouts:
- `item_student.xml`: Student list item
- `item_message.xml`: Message list item
- `custom_info_window.xml`: Map marker info window

### 3.2 Resource Files

#### 1. Strings (`res/values/strings.xml`)
- App text content
- Error messages
- Button labels
- Toast messages

#### 2. Drawables (`res/drawable/`)
- `ic_bus.xml`: Bus icon
- `ic_location.xml`: Location marker
- `salu_logo.xml`: University logo
- Various status icons and backgrounds

#### 3. Colors (`res/values/colors.xml`)
- Primary colors
- Status colors
- Text colors

## 4. Key Features and Modification Points

### 4.1 Location Tracking
- **Configuration:** `DriverDashboardActivity.kt`
- **Update interval:** Line ~150
- **Distance threshold:** Line ~160
- **Location accuracy:** Line ~155

### 4.2 Map Configuration
- **`MapActivity.kt`:**
  - Zoom levels: Lines ~195-200
