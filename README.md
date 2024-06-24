# Ez-Chat 💬
#### Video Demo: https://youtu.be/EYpkZi3A0DY
#### Description:
This is my CS50x Final Project - Ez-Chat, it is interactive and responsive web chatting app. I used packages Flask and Socket.IO to create the responsive chat platform. Users can join existing chat rooms or create new ones and the messages get update in real time. This README file provides a comprehensive overview of the project, including its structure, features, design and instructions for running the application.

## ***[Temporary Link](https://ezchat-ctqo6zafca-as.a.run.app/)***
## ***[Temporary Link 2](https://vikaskumar.live/)***
### Screenshots:
![1](ezchat1.png)
![2](ezchat2.png)

### Features
- **Real-time Messaging:** Ez-Chat uses Socket.IO to give real time messaging experience. Users in the same chat room can send and receive messages instantly without the need to refresh the page.
- **Room Management:** EZ-Chat allows users to join existing chat rooms using a unique 4 character long room code or create new chat room. Whenever you make a room, it generates a unique 4 character long code for that room only.
  Also once everyone leaves, the room gets deleted.
- **User Notifications:** While inside a room, everyone gets notified whenever a new member joins or someone leaves, with their respective timestamps.
- **Universal Design:** The app works smoothly on all devices including PC, Mobile, Tab, etc.

### Project Structure

#### 1. `app.py`
The main Flask application file, `app.py`, handles routing, session management and integrates Flask with Socket.IO for real time chatting. Key functionalities:
- **Home Route (`/`):** Renders the homepage where users can enter their name and room code to join or create a chat room.
  
- **Room Route (`/room`):** Displays the chat room for the specified room code.
  
- **Socket.IO Events:** Manages events such as sending messages, joining rooms and handles disconnections. The server-side events ensure messages are broadcast to all users in the room.

#### 2. `templates/`
This directory contains the HTML templates used in the project. Jinja2 is used to render dynamic content on the various html pages in this directory.
- **`base.html`:** It contains overall layout of the web app which we will use to extend on other html pages using jinja2 syntax.
  
- **`home.html`:** The homepage template where users can join with unique code or create their own chat rooms. It includes a form for entering a name and room code, along with buttons to join or create a room.
  
- **`room.html`:** The chat room template shows the input box, send button and the canvas where messages get shown to all the users in that particular room and also for them to write new messages.

#### 3. `static/css/`
This directory contains the CSS files for styling the app in order to stylize the app and make it appealing
- **`style.css`:** Defines the layout and design of the chat application, including message boxes, input fields, and overall page structure. It ensures the application looks consistent across different devices and screen sizes.
  
- **`bg.css`:** Contains the stunning background animations and the minute details of font size/site zoom size with respect to the screen size the app is opened in.

### Design Choices
- **Flask with Socket.IO:** Flask was chosen for its simplicity and ease of integration with Socket.IO, which is essential for real-time communication. This combination allows for efficient handling of HTTP requests and WebSocket connections.
  
- **Unique Room Codes:** To ensure privacy and avoid conflicts, a function generates unique 4-letter room codes. This design choice simplifies the process of joining and managing chat rooms.
  
- **Responsive Design:** The use of Bootstrap and custom CSS ensures that the application is usable on various devices, providing a seamless experience whether on a desktop or mobile. This design choice was made to cater to a wider audience and enhance usability.

### How to Run the Project
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/vikaskumar-23/EzChat.git
   cd EzChat
   ```
2. **Install Dependencies:**
   Ensure you have Python and pip installed, then run:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Application:**
   ```bash
   python app.py
   ```
   Open your browser and navigate to `http://127.0.0.1:5000` to access the chat application.

### Future Improvements
- **User Authentication:** Implementing user login and registration for a more personalized experience would enhance security and allow users to maintain their chat history.
- **Enhanced UI/UX:** Further refining the design to make the interface more intuitive and visually appealing can improve user engagement. This includes adding features like themes and customizations.
- **Additional Features:** Adding functionalities such as file sharing, emojis, and notifications for new messages can make the chat application more versatile and user-friendly. These features would provide a richer communication experience.

### Conclusion
Ez-Chat demonstrates the effective use of Flask and Socket.IO to create a functional and interactive real-time chat application. This project not only fulfills the requirements of the CS50x course but also provides a solid foundation for further development and enhancement. The blend of front-end and back-end technologies showcases a comprehensive understanding of web development principles and practices.

Feel free to explore, use, and contribute to the project. For any queries, you can reach me through [LinkedIn](https://www.linkedin.com/in/vikas-kumar-78584827b/), [YouTube](https://www.youtube.com/watch?v=dQw4w9WgXcQ), or [Instagram](https://www.instagram.com/currently_vikas).

---

