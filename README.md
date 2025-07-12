Faraz Mohammad - ayanalihaider9@gmail.com
Munish Upadhyay - munishupadhyay183@gmail.com
Siddhartha - singhsiddhartha220@gmail.com
Priyanshi - priyanshimaurya23@gmail.com

# ReWear - Community Clothing Exchange 👕♻️

A sustainable fashion platform that enables users to exchange unused clothing through direct swaps or a point-based redemption system, promoting textile waste reduction and circular fashion economy.

## 🌟 Features

### User Features
- **User Authentication**: Secure email/password registration and login system
- **Landing Page**: Engaging platform introduction with clear calls-to-action
- **Item Browsing**: Browse available clothing items with detailed information
- **Item Listing**: Upload and list your unused clothing items
- **Swap System**: Request direct swaps with other users
- **Points System**: Redeem clothing items using earned points
- **User Dashboard**: Track profile, points balance, and swap history
- **Item Management**: Monitor uploaded items and swap status

### Admin Features
- **Content Moderation**: Approve/reject item listings
- **Spam Prevention**: Remove inappropriate or spam items
- **Admin Panel**: Lightweight oversight dashboard

## 🛠️ Tech Stack

### Frontend
- **React.js** - UI library for building user interfaces
- **React Router** - Client-side routing
- **Axios** - HTTP client for API calls
- **CSS3/Styled Components** - Styling and responsive design

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database for data storage
- **Mongoose** - MongoDB object modeling

### Additional Technologies
- **JWT** - JSON Web Tokens for authentication
- **Multer** - File upload handling
- **Cloudinary** - Image storage and management
- **bcryptjs** - Password hashing
- **CORS** - Cross-origin resource sharing

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/rewear.git
   cd rewear
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Configuration**
   
   Create a `.env` file in the backend directory:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/rewear
   JWT_SECRET=your_jwt_secret_key
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

5. **Start the application**
   
   Backend (from backend directory):
   ```bash
   npm start
   ```
   
   Frontend (from frontend directory):
   ```bash
   npm start
   ```

6. **Access the application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`

## 📁 Project Structure

```
rewear/
├── backend/
│   ├── config/
│   │   └── db.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── itemController.js
│   │   ├── userController.js
│   │   └── swapController.js
│   ├── middleware/
│   │   ├── auth.js
│   │   ├── admin.js
│   │   └── upload.js
│   ├── models/
│   │   ├── User.js
│   │   ├── Item.js
│   │   └── Swap.js
│   ├── routes/
│   │   ├── auth.js
│   │   ├── items.js
│   │   ├── users.js
│   │   └── swaps.js
│   ├── utils/
│   │   └── cloudinary.js
│   └── server.js
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── common/
│   │   │   ├── auth/
│   │   │   ├── items/
│   │   │   ├── dashboard/
│   │   │   └── admin/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── utils/
│   │   └── App.js
│   └── package.json
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Items
- `GET /api/items` - Get all items
- `POST /api/items` - Create new item
- `GET /api/items/:id` - Get item details
- `PUT /api/items/:id` - Update item
- `DELETE /api/items/:id` - Delete item

### Swaps
- `POST /api/swaps` - Create swap request
- `GET /api/swaps/user` - Get user's swaps
- `PUT /api/swaps/:id` - Update swap status

### Admin
- `GET /api/admin/pending-items` - Get pending items
- `PUT /api/admin/approve-item/:id` - Approve item
- `DELETE /api/admin/reject-item/:id` - Reject item

## 🎨 Key Components

### Frontend Components
- **LandingPage**: Main entry point with featured items
- **ItemBrowser**: Browse and filter available items
- **ItemDetail**: Detailed item view with swap options
- **Dashboard**: User profile and activity overview
- **AddItem**: Form to list new items
- **AdminPanel**: Administrative controls

### Backend Models
- **User**: User accounts with points and profile data
- **Item**: Clothing items with details and images
- **Swap**: Swap transactions and history

## 🔐 Authentication & Security

- JWT-based authentication system
- Password hashing with bcrypt
- Protected routes for authenticated users
- Admin role-based access control
- Input validation and sanitization

## 📱 Responsive Design

ReWear is fully responsive and optimized for:
- Desktop computers
- Tablets
- Mobile devices

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with the MERN stack
- Inspired by sustainable fashion initiatives
- Thanks to the open-source community for tools and libraries

---

*ReWear - Making fashion sustainable, one swap at a time* 🌱
