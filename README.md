# Testing Simple Video Call Application

## 1. Start the Spring Boot Application
Run the backend with the following command:
```sh
mvn spring-boot:run
```
Ensure:
- ✅ WebSockets (Socket.io) are active  
- ✅ Keycloak authentication is working  
- ✅ No errors appear in the logs  

## 2. Ensure HTTPS Protocol
- HTTPS is required to enable browser permissions for camera and microphone.
- Verify that the backend is running on **`https://192.168.0.104:8443`**.

## 3. Connect Devices
### Notebook
1. Open: `https://192.168.0.104:8443`
2. Enter your **User ID** and press **Connect**.

### Mobile
1. Open: `https://192.168.0.104:8443`
2. Enter your **User ID** and press **Connect**.

## 4. Make a Video Call
- Enter the **Remote User ID**.
- Start the call.
- Confirm:
  - ✅ Video and audio are working  
  - ✅ Connection is stable  
  - ✅ WebRTC signaling is successful  

## 5. Debugging Issues
### Browser Console
- Open Developer Tools (F12 → Console/Network Tab) and check for WebRTC/WebSocket errors.

### Backend Logs
- Check Spring Boot logs for connection issues.

### STUN/TURN Server
- Ensure proper ICE candidate exchange for NAT traversal.

Let me know if you need further troubleshooting assistance! 🚀

