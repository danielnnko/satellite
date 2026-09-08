# Smart Hardware Dashboard

A Python/PySide6 desktop application for real-time smart hardware telemetry monitoring and GPS tracking. The system integrates **QWebEngineView** with **Leaflet.js** to visualize device locations on an interactive map.

## 🚀 Features

* Real-time hardware telemetry monitoring
* GPS latitude and longitude tracking
* Interactive Leaflet map
* Python and JavaScript integration
* PySide6 graphical user interface
* Embedded web content using QWebEngineView
* Automatic device position updates
* Safe handling of asynchronous map initialization
* Expandable architecture for IoT hardware integration

## 🛠️ Technologies

* **Python 3**
* **PySide6**
* **Qt WebEngine**
* **HTML5**
* **CSS3**
* **JavaScript**
* **Leaflet.js**
* **Git & GitHub**

## 📂 Project Structure

```text
smart-hardware-dashboard/
│
├── main.py
├── map.html
├── requirements.txt
├── README.md
├── .gitignore
│
└── assets/
    ├── images/
    └── icons/
```

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/smart-hardware-dashboard.git
```

Enter the project directory:

```bash
cd smart-hardware-dashboard
```

Create a Python virtual environment:

```bash
python3 -m venv venv
```

Activate the environment:

```bash
source venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Run the Application

```bash
python main.py
```

## 📍 GPS Tracking

The dashboard receives latitude and longitude coordinates and sends them to the embedded Leaflet map.

Example:

```python
update_position(latitude, longitude)
```

The map is updated using JavaScript:

```javascript
if (typeof map !== 'undefined' && typeof marker !== 'undefined') {
    map.setView([lat, lon], 13);
    marker.setLatLng([lat, lon]);
}
```

This prevents JavaScript errors when the map has not finished initializing.

## 🔄 System Data Flow

```text
Smart Hardware / GPS
        │
        ▼
Telemetry Data
        │
        ▼
Python Application
        │
        ▼
PySide6 Dashboard
        │
        ▼
QWebEngineView
        │
        ▼
Leaflet.js Map
        │
        ▼
Real-Time Device Location
```

## 🔮 Future Improvements

* ESP32 and Arduino integration
* Real GPS hardware
* MQTT communication
* REST API
* WebSocket telemetry
* Database integration
* Multiple-device tracking
* Temperature and humidity monitoring
* Battery monitoring
* Speed monitoring
* Historical location tracking
* IoT cloud integration
* Authentication and authorization

## 🧪 Testing

Check the Python source code for syntax errors:

```bash
python -m py_compile main.py
```

## 👨‍💻 Author

**Daniel Joshua Nnko**

Computer Engineering

Tanzania

## 📜 License

This project is licensed under the MIT License.
