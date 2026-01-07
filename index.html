import React, { useState, useEffect } from 'react';
import { ShoppingCart, Search, Heart, Star, Filter, X, Menu, Plus, Upload, User, Settings, LogOut, Edit3, Trash2, CheckCircle, MessageCircle, MapPin, Bell, Share2, Clock, Calendar, Sun, CloudRain, Leaf, Flower } from 'lucide-react';

// Mock product data with sellers
const initialProducts = [
  {
    id: 1,
    name: "Classic White T-Shirt",
    price: 2500,
    discount: 10,
    category: "Tops",
    image: "https://placehold.co/300x400/e2e8f0/64748b?text=White+T-Shirt",
    rating: 4.5,
    reviews: 128,
    inStock: true,
    featured: true,
    colors: ["White", "Black", "Gray"],
    sizes: ["S", "M", "L", "XL"],
    sellerId: 1,
    seller: {
      name: "Jane's Boutique",
      rating: 4.8,
      joined: "2025-03-15"
    }
  },
  {
    id: 2,
    name: "Denim Slim Fit Jeans",
    price: 6500,
    discount: 15,
    category: "Bottoms",
    image: "https://placehold.co/300x400/475569/ffffff?text=Denim+Jeans",
    rating: 4.7,
    reviews: 256,
    inStock: true,
    featured: true,
    colors: ["Blue", "Black"],
    sizes: ["28", "30", "32", "34", "36"],
    sellerId: 2,
    seller: {
      name: "Fashion Hub Nairobi",
      rating: 4.9,
      joined: "2024-11-20"
    }
  },
  {
    id: 3,
    name: "Casual Button-Down Shirt",
    price: 3800,
    discount: 0,
    category: "Tops",
    image: "https://placehold.co/300x400/f1f5f9/0f172a?text=Button+Down",
    rating: 4.3,
    reviews: 89,
    inStock: true,
    featured: false,
    colors: ["Navy", "White", "Beige"],
    sizes: ["S", "M", "L", "XL"],
    sellerId: 1,
    seller: {
      name: "Jane's Boutique",
      rating: 4.8,
      joined: "2025-03-15"
    }
  },
  {
    id: 4,
    name: "Premium Hoodie",
    price: 4800,
    discount: 20,
    category: "Outerwear",
    image: "https://placehold.co/300x400/1e293b/ffffff?text=Hoodie",
    rating: 4.8,
    reviews: 312,
    inStock: true,
    featured: true,
    colors: ["Gray", "Black", "Burgundy"],
    sizes: ["S", "M", "L", "XL", "XXL"],
    sellerId: 3,
    seller: {
      name: "Urban Streetwear",
      rating: 4.6,
      joined: "2025-01-08"
    }
  },
  {
    id: 5,
    name: "Summer Dress",
    price: 5200,
    discount: 25,
    category: "Dresses",
    image: "https://placehold.co/300x400/fef3c7/d97706?text=Summer+Dress",
    rating: 4.6,
    reviews: 174,
    inStock: true,
    featured: false,
    colors: ["Yellow", "Floral", "White"],
    sizes: ["XS", "S", "M", "L"],
    sellerId: 4,
    seller: {
      name: "Sunny Styles",
      rating: 4.5,
      joined: "2025-04-01"
    }
  },
  {
    id: 6,
    name: "Leather Jacket",
    price: 12500,
    discount: 5,
    category: "Outerwear",
    image: "https://placehold.co/300x400/0f172a/f1f5f9?text=Leather+Jacket",
    rating: 4.9,
    reviews: 87,
    inStock: true,
    featured: true,
    colors: ["Black", "Brown"],
    sizes: ["S", "M", "L"],
    sellerId: 2,
    seller: {
      name: "Fashion Hub Nairobi",
      rating: 4.9,
      joined: "2024-11-20"
    }
  }
];

const initialSellers = [
  {
    id: 1,
    name: "Jane's Boutique",
    email: "jane@example.com",
    phone: "+254 712 345 678",
    location: "Nairobi",
    rating: 4.8,
    joined: "2025-03-15",
    paymentMethod: "Paybill",
    paymentDetails: "123456",
    products: [1, 3],
    followers: [],
    following: [],
    messagesEnabled: [],
    deliveryLocations: ["Nairobi CBD", "Westlands", "Karen"]
  },
  {
    id: 2,
    name: "Fashion Hub Nairobi",
    email: "info@fashionhub.co.ke",
    phone: "+254 723 456 789",
    location: "Westlands, Nairobi",
    rating: 4.9,
    joined: "2024-11-20",
    paymentMethod: "Till Number",
    paymentDetails: "987654",
    products: [2, 6],
    followers: [],
    following: [],
    messagesEnabled: [],
    deliveryLocations: ["Nairobi", "Kiambu", "Machakos"]
  },
  {
    id: 3,
    name: "Urban Streetwear",
    email: "contact@urbanstreet.co.ke",
    phone: "+254 734 567 890",
    location: "Mombasa Road, Nairobi",
    rating: 4.6,
    joined: "2025-01-08",
    paymentMethod: "Send Money",
    paymentDetails: "+254 734 567 890",
    products: [4],
    followers: [],
    following: [],
    messagesEnabled: [],
    deliveryLocations: ["Nairobi", "Thika", "Ruiru"]
  },
  {
    id: 4,
    name: "Sunny Styles",
    email: "hello@sunnystyles.co.ke",
    phone: "+254 745 678 901",
    location: "Kilimani, Nairobi",
    rating: 4.5,
    joined: "2025-04-01",
    paymentMethod: "Paybill",
    paymentDetails: "456789",
    products: [5],
    followers: [],
    following: [],
    messagesEnabled: [],
    deliveryLocations: ["Nairobi", "Ngong", "Kikuyu"]
  }
];

// Kenyan seasonal themes
const getSeasonalTheme = () => {
  const now = new Date();
  const month = now.getMonth(); // 0-11 (Jan-Dec)
  
  // Kenyan seasons:
  // Dec-Feb: Short dry season (hot & dry) - Summer theme
  // Mar-May: Long rains (wet season) - Rainy theme
  // Jun-Oct: Long dry season (cool & dry) - Dry season theme
  // Nov: Short rains (wet season) - Short rains theme
  
  if (month >= 11 || month <= 1) {
    // December, January, February - Short dry season
    return {
      name: "Short Dry Season",
      bgColor: "from-orange-100 to-yellow-100",
      accentColor: "from-orange-500 to-yellow-500",
      textColor: "text-orange-800",
      icon: Sun,
      description: "Hot & Dry Season",
      graphics: [
        "https://placehold.co/200x100/fdb813/ffffff?text=☀️+Hot+Weather",
        "https://placehold.co/200x100/f59e0b/ffffff?text=🌾+Harvest+Time"
      ]
    };
  } else if (month >= 2 && month <= 4) {
    // March, April, May - Long rains
    return {
      name: "Long Rains",
      bgColor: "from-blue-100 to-cyan-100",
      accentColor: "from-blue-500 to-cyan-500",
      textColor: "text-blue-800",
      icon: CloudRain,
      description: "Rainy Season",
      graphics: [
        "https://placehold.co/200x100/3b82f6/ffffff?text=🌧️+Long+Rains",
        "https://placehold.co/200x100/06b6d4/ffffff?text=🌱+Green+Growth"
      ]
    };
  } else if (month >= 5 && month <= 9) {
    // June to September - Long dry season
    return {
      name: "Long Dry Season",
      bgColor: "from-amber-100 to-amber-200",
      accentColor: "from-amber-500 to-amber-600",
      textColor: "text-amber-800",
      icon: Leaf,
      description: "Cool & Dry Season",
      graphics: [
        "https://placehold.co/200x100/f59e0b/ffffff?text=🍂+Dry+Season",
        "https://placehold.co/200x100/d97706/ffffff?text=🌾+Harvest+Time"
      ]
    };
  } else {
    // October, November - Short rains
    return {
      name: "Short Rains",
      bgColor: "from-green-100 to-emerald-100",
      accentColor: "from-green-500 to-emerald-500",
      textColor: "text-green-800",
      icon: Flower,
      description: "Short Rains Season",
      graphics: [
        "https://placehold.co/200x100/10b981/ffffff?text=🌸+Short+Rains",
        "https://placehold.co/200x100/059669/ffffff?text=🌿+Flowering+Season"
      ]
    };
  }
};

export default function App() {
  const [products, setProducts] = useState(initialProducts);
  const [sellers, setSellers] = useState(initialSellers);
  const [cartItems, setCartItems] = useState([]);
  const [wishlist, setWishlist] = useState([]);
  const [searchQuery, setSearchQuery] = useState("");
  const [selectedCategory, setSelectedCategory] = useState("All");
  const [mobileMenuOpen, setMobileMenuOpen] = useState(false);
  const [showFilters, setShowFilters] = useState(false);
  const [user, setUser] = useState(null);
  const [currentView, setCurrentView] = useState("browse");
  const [newSeller, setNewSeller] = useState({
    name: "",
    email: "",
    phone: "",
    location: "",
    paymentMethod: "Paybill",
    paymentDetails: ""
  });
  const [newProduct, setNewProduct] = useState({
    name: "",
    price: "",
    discount: "0",
    category: "Tops",
    description: "",
    colors: "",
    sizes: "",
    image: ""
  });
  const [notifications, setNotifications] = useState([]);
  const [messages, setMessages] = useState([]);
  const [followRequests, setFollowRequests] = useState([]);
  const [seasonalTheme, setSeasonalTheme] = useState(getSeasonalTheme());

  // Update seasonal theme periodically
  useEffect(() => {
    const timer = setInterval(() => {
      setSeasonalTheme(getSeasonalTheme());
    }, 300000); // Update every 5 minutes
    return () => clearInterval(timer);
  }, []);

  // Filter products based on search and category
  const filteredProducts = products.filter(product => {
    const matchesSearch = product.name.toLowerCase().includes(searchQuery.toLowerCase());
    const matchesCategory = selectedCategory === "All" || product.category === selectedCategory;
    return matchesSearch && matchesCategory;
  });

  // Get seller's products
  const getSellerProducts = () => {
    if (!user) return [];
    return products.filter(product => product.sellerId === user.id);
  };

  // Add to cart function
  const addToCart = (product) => {
    setCartItems(prev => {
      const existing = prev.find(item => item.id === product.id);
      if (existing) {
        return prev.map(item => 
          item.id === product.id 
            ? { ...item, quantity: item.quantity + 1 } 
            : item
        );
      }
      return [...prev, { ...product, quantity: 1 }];
    });
  };

  // Toggle wishlist
  const toggleWishlist = (productId) => {
    setWishlist(prev => 
      prev.includes(productId) 
        ? prev.filter(id => id !== productId)
        : [...prev, productId]
    );
  };

  // Follow seller
  const followSeller = (sellerId) => {
    if (!user) {
      // Show login/signup prompt
      return;
    }
    
    // Check if already following
    const seller = sellers.find(s => s.id === sellerId);
    if (seller.followers.includes(user.id)) {
      // Unfollow
      setSellers(prev => 
        prev.map(s => 
          s.id === sellerId 
            ? { ...s, followers: s.followers.filter(id => id !== user.id) }
            : s
        )
      );
      return;
    }
    
    // Send follow request
    setFollowRequests(prev => [...prev, { 
      id: Date.now(), 
      buyerId: user.id, 
      sellerId, 
      status: "pending",
      timestamp: new Date().toISOString()
    }]);
    
    // Show notification
    setNotifications(prev => [
      ...prev,
      {
        id: Date.now(),
        type: "follow",
        message: `Follow request sent to ${seller.name}`,
        timestamp: new Date().toISOString(),
        read: false
      }
    ]);
  };

  // Accept follow request
  const acceptFollowRequest = (requestId) => {
    const request = followRequests.find(r => r.id === requestId);
    if (!request) return;
    
    setSellers(prev => 
      prev.map(s => 
        s.id === request.sellerId 
          ? { ...s, followers: [...s.followers, request.buyerId] }
          : s
      )
    );
    
    setFollowRequests(prev => prev.filter(r => r.id !== requestId));
    
    // Notify buyer
    setNotifications(prev => [
      ...prev,
      {
        id: Date.now(),
        type: "follow-accepted",
        message: `You are now following ${sellers.find(s => s.id === request.sellerId).name}`,
        timestamp: new Date().toISOString(),
        read: false
      }
    ]);
  };

  // Send message
  const sendMessage = (sellerId, message) => {
    const seller = sellers.find(s => s.id === sellerId);
    if (!seller.messagesEnabled.includes(user.id)) {
      setNotifications(prev => [
        ...prev,
        {
          id: Date.now(),
          type: "error",
          message: `${seller.name} has not enabled messages from you. You need to follow them first.`,
          timestamp: new Date().toISOString(),
          read: false
        }
      ]);
      return;
    }
    
    const newMessage = {
      id: Date.now(),
      from: user.id,
      to: sellerId,
      message,
      timestamp: new Date().toISOString(),
      read: false
    };
    
    setMessages(prev => [...prev, newMessage]);
    
    setNotifications(prev => [
      ...prev,
      {
        id: Date.now() + 1,
        type: "message",
        message: `Message sent to ${seller.name}`,
        timestamp: new Date().toISOString(),
        read: false
      }
    ]);
  };

  // Create new seller account
  const handleCreateSeller = () => {
    const sellerId = sellers.length + 1;
    const newSellerData = {
      ...newSeller,
      id: sellerId,
      rating: 0,
      joined: new Date().toISOString().split('T')[0],
      products: [],
      followers: [],
      following: [],
      messagesEnabled: [],
      deliveryLocations: [newSeller.location]
    };
    
    setSellers(prev => [...prev, newSellerData]);
    setUser(newSellerData);
    setCurrentView("seller-dashboard");
    setNewSeller({
      name: "",
      email: "",
      phone: "",
      location: "",
      paymentMethod: "Paybill",
      paymentDetails: ""
    });
  };

  // Create new product
  const handleCreateProduct = () => {
    const productId = products.length + 1;
    const productData = {
      id: productId,
      ...newProduct,
      price: parseFloat(newProduct.price),
      discount: parseInt(newProduct.discount) || 0,
      originalPrice: parseFloat(newProduct.price),
      rating: 0,
      reviews: 0,
      inStock: true,
      featured: false,
      colors: newProduct.colors.split(',').map(c => c.trim()),
      sizes: newProduct.sizes.split(',').map(s => s.trim()),
      sellerId: user.id,
      seller: {
        name: user.name,
        rating: user.rating,
        joined: user.joined
      }
    };
    
    setProducts(prev => [...prev, productData]);
    
    // Update seller's products
    setSellers(prev => 
      prev.map(seller => 
        seller.id === user.id 
          ? { ...seller, products: [...seller.products, productId] }
          : seller
      )
    );
    
    // Notify followers
    if (user.followers.length > 0) {
      user.followers.forEach(followerId => {
        setNotifications(prev => [
          ...prev,
          {
            id: Date.now() + followerId,
            type: "new-product",
            message: `${user.name} just added "${newProduct.name}" to their store!`,
            timestamp: new Date().toISOString(),
            read: false,
            productId: productId
          }
        ]);
      });
    }
    
    setNewProduct({
      name: "",
      price: "",
      discount: "0",
      category: "Tops",
      description: "",
      colors: "",
      sizes: "",
      image: ""
    });
    setCurrentView("seller-dashboard");
  };

  // Delete product
  const deleteProduct = (productId) => {
    setProducts(prev => prev.filter(p => p.id !== productId));
    setSellers(prev => 
      prev.map(seller => 
        seller.id === user.id 
          ? { ...seller, products: seller.products.filter(id => id !== productId) }
          : seller
      )
    );
  };

  // Enable messages from buyer
  const enableMessagesFromBuyer = (buyerId) => {
    setSellers(prev => 
      prev.map(seller => 
        seller.id === user.id 
          ? { ...seller, messagesEnabled: [...seller.messagesEnabled, buyerId] }
          : seller
      )
    );
  };

  // Calculate cart totals
  const cartTotal = cartItems.reduce((total, item) => total + (item.price * (1 - (item.discount || 0) / 100) * item.quantity), 0);
  const cartCount = cartItems.reduce((count, item) => count + item.quantity, 0);

  // Logout
  const handleLogout = () => {
    setUser(null);
    setCurrentView("browse");
  };

  // Get seller by ID
  const getSellerById = (id) => sellers.find(s => s.id === id);

  // Check if user is following seller
  const isFollowing = (sellerId) => {
    if (!user) return false;
    const seller = getSellerById(sellerId);
    return seller && seller.followers.includes(user.id);
  };

  // Check if messages are enabled
  const canMessage = (sellerId) => {
    if (!user) return false;
    const seller = getSellerById(sellerId);
    return seller && seller.messagesEnabled.includes(user.id);
  };

  // Check if follow request exists
  const hasPendingFollowRequest = (sellerId) => {
    if (!user) return false;
    return followRequests.some(r => r.buyerId === user.id && r.sellerId === sellerId && r.status === "pending");
  };

  return (
    <div className={`min-h-screen bg-gradient-to-br ${seasonalTheme.bgColor}`}>
      {/* Google Fonts import for Bloomin Gflow */}
      <style jsx global>{`
        @import url('https://fonts.googleapis.com/css2?family=Bloomin+Gflow&display=swap');
      `}</style>

      {/* Header */}
      <header className="bg-white shadow-sm sticky top-0 z-50">
        <div className="container mx-auto px-4">
          <div className="flex items-center justify-between h-16">
            {/* Logo */}
            <div className="flex items-center space-x-2">
              <div className="w-8 h-8 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full"></div>
              <span className="text-xl font-bold text-gray-900 font-['Bloomin_Gflow'] text-2xl tracking-wide">
                Online Gikomba
              </span>
              <span className={`ml-2 px-2 py-1 rounded-full text-xs font-bold ${seasonalTheme.textColor} bg-white`}>
                {seasonalTheme.name}
              </span>
            </div>

            {/* Desktop Navigation */}
            <nav className="hidden md:flex space-x-8">
              <button 
                onClick={() => setCurrentView("browse")}
                className="text-gray-700 hover:text-blue-600 font-medium"
              >
                Browse
              </button>
              <button 
                onClick={() => setCurrentView("create-seller")}
                className="text-gray-700 hover:text-blue-600 font-medium"
              >
                Sell
              </button>
            </nav>

            {/* User Actions */}
            <div className="flex items-center space-x-4">
              {user ? (
                <div className="flex items-center space-x-2">
                  <button 
                    onClick={() => setNotifications(prev => prev.map(n => ({ ...n, read: true })))}
                    className="p-2 text-gray-600 hover:text-blue-600 relative"
                  >
                    <Bell className="w-5 h-5" />
                    {notifications.filter(n => !n.read).length > 0 && (
                      <span className="absolute -top-1 -right-1 bg-red-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">
                        {notifications.filter(n => !n.read).length}
                      </span>
                    )}
                  </button>
                  <div className="w-8 h-8 bg-blue-500 rounded-full flex items-center justify-center text-white font-bold text-sm">
                    {user.name.charAt(0)}
                  </div>
                  <button 
                    onClick={() => setCurrentView("seller-dashboard")}
                    className="p-2 text-gray-600 hover:text-blue-600"
                  >
                    <Settings className="w-5 h-5" />
                  </button>
                  <button 
                    onClick={handleLogout}
                    className="p-2 text-gray-600 hover:text-red-600"
                  >
                    <LogOut className="w-5 h-5" />
                  </button>
                </div>
              ) : (
                <>
                  <button 
                    onClick={() => setCurrentView("create-seller")}
                    className="hidden md:flex items-center space-x-1 bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-lg font-medium"
                  >
                    <Plus className="w-4 h-4" />
                    <span>Sell</span>
                  </button>
                  <button className="p-2 text-gray-600 hover:text-blue-600 relative">
                    <Heart className="w-5 h-5" />
                    {wishlist.length > 0 && (
                      <span className="absolute -top-1 -right-1 bg-red-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">
                        {wishlist.length}
                      </span>
                    )}
                  </button>
                  <div className="relative">
                    <button className="p-2 text-gray-600 hover:text-blue-600 relative">
                      <ShoppingCart className="w-5 h-5" />
                      {cartCount > 0 && (
                        <span className="absolute -top-1 -right-1 bg-blue-600 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">
                          {cartCount}
                        </span>
                      )}
                    </button>
                  </div>
                </>
              )}

              <button className="md:hidden p-2 text-gray-600">
                <Menu className="w-6 h-6" onClick={() => setMobileMenuOpen(true)} />
              </button>
            </div>
          </div>

          {/* Mobile Menu */}
          {mobileMenuOpen && (
            <div className="md:hidden absolute top-16 left-0 right-0 bg-white shadow-lg z-50">
              <div className="p-4 space-y-4">
                <div className="flex justify-between items-center">
                  <h3 className="font-semibold text-gray-900 font-['Bloomin_Gflow']">Menu</h3>
                  <button onClick={() => setMobileMenuOpen(false)}>
                    <X className="w-5 h-5" />
                  </button>
                </div>
                <div className="relative">
                  <Search className="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400 w-4 h-4" />
                  <input
                    type="text"
                    placeholder="Search products..."
                    className="w-full pl-10 pr-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                    value={searchQuery}
                    onChange={(e) => setSearchQuery(e.target.value)}
                  />
                </div>
                <nav className="space-y-2">
                  <button 
                    onClick={() => { setCurrentView("browse"); setMobileMenuOpen(false); }}
                    className="block py-2 text-gray-700 hover:text-blue-600 font-medium"
                  >
                    Browse
                  </button>
                  <button 
                    onClick={() => { setCurrentView("create-seller"); setMobileMenuOpen(false); }}
                    className="block py-2 text-gray-700 hover:text-blue-600 font-medium"
                  >
                    Sell
                  </button>
                </nav>
              </div>
            </div>
          )}
        </div>
      </header>

      {/* Seasonal Banner */}
      <section className={`py-4 text-center ${seasonalTheme.textColor}`}>
        <div className="container mx-auto px-4 flex items-center justify-center space-x-4">
          <seasonalTheme.icon className="w-6 h-6" />
          <span className="font-semibold">{seasonalTheme.description}</span>
          <span>•</span>
          <span>Perfect for {seasonalTheme.name.toLowerCase()} fashion</span>
        </div>
      </section>

      {/* Seasonal Graphics */}
      <section className="py-2 bg-white">
        <div className="container mx-auto px-4">
          <div className="flex flex-wrap justify-center gap-4">
            {seasonalTheme.graphics.map((graphic, index) => (
              <div key={index} className="w-40 h-20">
                <img src={graphic} alt={`Seasonal graphic ${index + 1}`} className="w-full h-full object-cover rounded-lg" />
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Main Content */}
      <main className="py-8">
        {currentView === "browse" && (
          <>
            {/* Hero Banner */}
            <section className={`bg-gradient-to-r ${seasonalTheme.accentColor} text-white py-16`}>
              <div className="container mx-auto px-4 text-center">
                <h1 className="text-4xl md:text-6xl font-bold mb-4 font-['Bloomin_Gflow'] tracking-wide">
                  Online Gikomba
                </h1>
                <p className="text-xl md:text-2xl mb-8 max-w-3xl mx-auto">
                  Kenya's largest marketplace for fashion and clothing. Buy and sell clothes in Kenyan Shillings.
                </p>
                <div className="flex flex-col sm:flex-row gap-4 justify-center">
                  <button 
                    onClick={() => setCurrentView("create-seller")}
                    className="bg-white text-blue-700 hover:bg-gray-100 font-bold py-3 px-8 rounded-full text-lg transition-colors"
                  >
                    Sell Your Clothes
                  </button>
                  <button className="bg-transparent border-2 border-white text-white hover:bg-white/10 font-bold py-3 px-8 rounded-full text-lg transition-colors">
                    Browse Products
                  </button>
                </div>
              </div>
            </section>

            {/* Search and Filters */}
            <section className="py-6 bg-gray-200">
              <div className="container mx-auto px-4">
                <div className="flex flex-col md:flex-row gap-4">
                  <div className="flex-1 relative">
                    <Search className="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400 w-5 h-5" />
                    <input
                      type="text"
                      placeholder="Search for clothes, sellers, or categories..."
                      className="w-full pl-10 pr-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      value={searchQuery}
                      onChange={(e) => setSearchQuery(e.target.value)}
                    />
                  </div>
                  <select 
                    className="border border-gray-300 rounded-lg px-4 py-3 focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                    value={selectedCategory}
                    onChange={(e) => setSelectedCategory(e.target.value)}
                  >
                    <option value="All">All Categories</option>
                    <option value="Tops">Tops</option>
                    <option value="Bottoms">Bottoms</option>
                    <option value="Dresses">Dresses</option>
                    <option value="Outerwear">Outerwear</option>
                    <option value="Accessories">Accessories</option>
                    <option value="Shoes">Shoes</option>
                  </select>
                </div>
              </div>
            </section>

            {/* Products Grid */}
            <section className="py-8">
              <div className="container mx-auto px-4">
                {filteredProducts.length === 0 ? (
                  <div className="text-center py-12">
                    <div className="text-6xl mb-4">🔍</div>
                    <h3 className="text-xl font-semibold text-gray-900 mb-2 font-['Bloomin_Gflow']">
                      No products found
                    </h3>
                    <p className="text-gray-600 mb-4">Try adjusting your search or filter criteria</p>
                  </div>
                ) : (
                  <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
                    {filteredProducts.map((product) => (
                      <div key={product.id} className="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow duration-300">
                        <div className="relative">
                          <img 
                            src={product.image} 
                            alt={product.name}
                            className="w-full h-64 object-cover"
                          />
                          {!product.inStock && (
                            <div className="absolute top-4 left-4 bg-red-500 text-white px-2 py-1 rounded text-sm font-medium">
                              Out of Stock
                            </div>
                          )}
                          {product.discount > 0 && (
                            <div className="absolute top-4 right-4 bg-red-500 text-white px-2 py-1 rounded text-sm font-medium">
                              {product.discount}% OFF
                            </div>
                          )}
                          <button
                            onClick={() => toggleWishlist(product.id)}
                            className={`absolute top-4 right-4 p-2 rounded-full ${
                              wishlist.includes(product.id) 
                                ? 'bg-red-500 text-white' 
                                : 'bg-white text-gray-600 hover:text-red-500'
                            }`}
                          >
                            <Heart className="w-4 h-4" fill={wishlist.includes(product.id) ? "currentColor" : "none"} />
                          </button>
                        </div>
                        
                        <div className="p-4">
                          <h3 className="font-semibold text-gray-900 mb-2">{product.name}</h3>
                          
                          <div className="mb-3">
                            <div className="flex items-center justify-between mb-2">
                              <span className="bg-blue-100 text-blue-800 text-xs font-medium px-2 py-1 rounded">
                                {product.seller.name}
                              </span>
                              <button
                                onClick={() => followSeller(product.sellerId)}
                                className={`flex items-center space-x-1 px-2 py-1 rounded text-xs font-medium ${
                                  isFollowing(product.sellerId)
                                    ? 'bg-green-100 text-green-800 hover:bg-green-200'
                                    : hasPendingFollowRequest(product.sellerId)
                                      ? 'bg-yellow-100 text-yellow-800'
                                      : 'bg-gray-100 text-gray-800 hover:bg-gray-200'
                                }`}
                              >
                                {isFollowing(product.sellerId) ? (
                                  <>
                                    <CheckCircle className="w-3 h-3" />
                                    <span>Following</span>
                                  </>
                                ) : hasPendingFollowRequest(product.sellerId) ? (
                                  <>
                                    <Clock className="w-3 h-3" />
                                    <span>Pending</span>
                                  </>
                                ) : (
                                  <>
                                    <User className="w-3 h-3" />
                                    <span>Follow</span>
                                  </>
                                )}
                              </button>
                            </div>
                            
                            <div className="flex items-center mb-2">
                              <div className="flex">
                                {[...Array(5)].map((_, i) => (
                                  <Star 
                                    key={i} 
                                    className={`w-4 h-4 ${
                                      i < Math.floor(product.rating) 
                                        ? 'text-yellow-400 fill-current' 
                                        : 'text-gray-300'
                                    }`}
                                  />
                                ))}
                              </div>
                              <span className="text-sm text-gray-600 ml-2">({product.reviews})</span>
                            </div>
                          </div>
                          
                          <div className="flex items-center justify-between mb-3">
                            <div>
                              {product.discount > 0 ? (
                                <>
                                  <span className="text-lg font-bold text-gray-900">
                                    Ksh {(product.price * (1 - product.discount/100)).toLocaleString()}
                                  </span>
                                  <span className="text-sm text-gray-500 line-through ml-2">
                                    Ksh {product.price.toLocaleString()}
                                  </span>
                                </>
                              ) : (
                                <span className="text-lg font-bold text-gray-900">
                                  Ksh {product.price.toLocaleString()}
                                </span>
                              )}
                            </div>
                            <span className="text-xs bg-orange-100 text-orange-800 px-2 py-1 rounded">
                              Save Ksh {(product.price * product.discount/100).toLocaleString()}
                            </span>
                          </div>
                          
                          <button
                            onClick={() => addToCart(product)}
                            disabled={!product.inStock}
                            className={`w-full py-2 px-4 rounded-lg font-medium transition-colors ${
                              product.inStock
                                ? 'bg-blue-600 hover:bg-blue-700 text-white'
                                : 'bg-gray-300 text-gray-500 cursor-not-allowed'
                            }`}
                          >
                            {product.inStock ? 'Add to Cart' : 'Out of Stock'}
                          </button>
                        </div>
                      </div>
                    ))}
                  </div>
                )}
              </div>
            </section>
          </>
        )}

        {currentView === "create-seller" && (
          <section className="py-12">
            <div className="max-w-4xl mx-auto px-4">
              <div className="bg-white rounded-xl shadow-lg p-8">
                <div className="text-center mb-8">
                  <div className="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                    <User className="w-8 h-8 text-blue-600" />
                  </div>
                  <h2 className="text-3xl font-bold text-gray-900 font-['Bloomin_Gflow'] mb-2">
                    Create Your Seller Account
                  </h2>
                  <p className="text-gray-600">
                    Join Online Gikomba and start selling your clothes to thousands of customers
                  </p>
                </div>

                <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Business Name *
                    </label>
                    <input
                      type="text"
                      value={newSeller.name}
                      onChange={(e) => setNewSeller({...newSeller, name: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="e.g., Jane's Boutique"
                    />
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Email Address *
                    </label>
                    <input
                      type="email"
                      value={newSeller.email}
                      onChange={(e) => setNewSeller({...newSeller, email: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="your@email.com"
                    />
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Phone Number *
                    </label>
                    <input
                      type="tel"
                      value={newSeller.phone}
                      onChange={(e) => setNewSeller({...newSeller, phone: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="+254 712 345 678"
                    />
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Location *
                    </label>
                    <input
                      type="text"
                      value={newSeller.location}
                      onChange={(e) => setNewSeller({...newSeller, location: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="e.g., Nairobi, Westlands"
                    />
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Payment Method *
                    </label>
                    <select
                      value={newSeller.paymentMethod}
                      onChange={(e) => setNewSeller({...newSeller, paymentMethod: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                    >
                      <option value="Paybill">M-Pesa Paybill</option>
                      <option value="Till Number">M-Pesa Till Number</option>
                      <option value="Send Money">M-Pesa Send Money</option>
                    </select>
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      {newSeller.paymentMethod === "Paybill" && "Paybill Number *"}
                      {newSeller.paymentMethod === "Till Number" && "Till Number *"}
                      {newSeller.paymentMethod === "Send Money" && "Phone Number for Send Money *"}
                    </label>
                    <input
                      type="text"
                      value={newSeller.paymentDetails}
                      onChange={(e) => setNewSeller({...newSeller, paymentDetails: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder={
                        newSeller.paymentMethod === "Paybill" ? "e.g., 123456" :
                        newSeller.paymentMethod === "Till Number" ? "e.g., 987654" :
                        "e.g., +254 712 345 678"
                      }
                    />
                  </div>
                </div>

                <div className="mt-8 flex justify-center space-x-4">
                  <button
                    onClick={() => setCurrentView("browse")}
                    className="px-6 py-3 border border-gray-300 text-gray-700 rounded-lg hover:bg-gray-50 font-medium"
                  >
                    Cancel
                  </button>
                  <button
                    onClick={handleCreateSeller}
                    disabled={!newSeller.name || !newSeller.email || !newSeller.phone || !newSeller.location || !newSeller.paymentDetails}
                    className="px-6 py-3 bg-blue-600 text-white rounded-lg hover:bg-blue-700 font-medium disabled:opacity-50 disabled:cursor-not-allowed"
                  >
                    Create Account
                  </button>
                </div>
              </div>
            </div>
          </section>
        )}

        {currentView === "seller-dashboard" && user && (
          <section className="py-8">
            <div className="max-w-7xl mx-auto px-4">
              {/* Dashboard Header */}
              <div className="bg-white rounded-xl shadow-lg p-6 mb-8">
                <div className="flex flex-col md:flex-row md:items-center md:justify-between">
                  <div className="flex items-center space-x-4 mb-4 md:mb-0">
                    <div className="w-16 h-16 bg-blue-600 rounded-full flex items-center justify-center text-white font-bold text-xl">
                      {user.name.charAt(0)}
                    </div>
                    <div>
                      <h2 className="text-2xl font-bold text-gray-900 font-['Bloomin_Gflow']">{user.name}</h2>
                      <p className="text-gray-600">{user.location}</p>
                      <div className="flex items-center mt-2">
                        <div className="flex text-yellow-400">
                          {[...Array(5)].map((_, i) => (
                            <Star key={i} className={`w-4 h-4 ${i < Math.floor(user.rating) ? 'fill-current' : ''}`} />
                          ))}
                        </div>
                        <span className="ml-2 text-sm text-gray-600">({user.rating}/5)</span>
                        <span className="ml-4 text-sm text-gray-600">
                          Followers: {user.followers.length}
                        </span>
                      </div>
                    </div>
                  </div>
                  
                  <div className="flex space-x-3">
                    <button
                      onClick={() => setCurrentView("create-product")}
                      className="flex items-center space-x-2 bg-green-600 hover:bg-green-700 text-white px-4 py-2 rounded-lg font-medium"
                    >
                      <Plus className="w-4 h-4" />
                      <span>Add Product</span>
                    </button>
                    <button
                      onClick={handleLogout}
                      className="flex items-center space-x-2 bg-gray-600 hover:bg-gray-700 text-white px-4 py-2 rounded-lg font-medium"
                    >
                      <LogOut className="w-4 h-4" />
                      <span>Logout</span>
                    </button>
                  </div>
                </div>
                
                {/* Payment & Delivery Info */}
                <div className="mt-6 grid grid-cols-1 lg:grid-cols-2 gap-6">
                  <div className="p-4 bg-blue-50 rounded-lg">
                    <h3 className="font-semibold text-gray-900 mb-2">Payment Information</h3>
                    <div className="grid grid-cols-2 gap-4">
                      <div>
                        <p className="text-sm text-gray-600">Method</p>
                        <p className="font-medium">{user.paymentMethod}</p>
                      </div>
                      <div>
                        <p className="text-sm text-gray-600">
                          {user.paymentMethod === "Paybill" && "Paybill Number"}
                          {user.paymentMethod === "Till Number" && "Till Number"}
                          {user.paymentMethod === "Send Money" && "Phone Number"}
                        </p>
                        <p className="font-medium">{user.paymentDetails}</p>
                      </div>
                    </div>
                  </div>
                  
                  <div className="p-4 bg-green-50 rounded-lg">
                    <h3 className="font-semibold text-gray-900 mb-2">Delivery Locations</h3>
                    <div className="flex flex-wrap gap-2">
                      {user.deliveryLocations.map((location, index) => (
                        <span key={index} className="px-3 py-1 bg-white text-green-800 rounded-full text-sm">
                          {location}
                        </span>
                      ))}
                    </div>
                    <button className="mt-2 flex items-center text-green-600 hover:text-green-800 text-sm">
                      <MapPin className="w-4 h-4 mr-1" />
                      Add/Update Locations
                    </button>
                  </div>
                </div>
                
                {/* Message Settings */}
                {user.followers.length > 0 && (
                  <div className="mt-6 p-4 bg-amber-50 rounded-lg">
                    <h3 className="font-semibold text-gray-900 mb-2">Message Permissions</h3>
                    <p className="text-sm text-gray-600 mb-3">
                      Manage who can send you messages. Only followers can request to message you.
                    </p>
                    <div className="space-y-2">
                      {user.followers.map(followerId => {
                        const follower = sellers.find(s => s.id === followerId) || { name: `User ${followerId}` };
                        return (
                          <div key={followerId} className="flex items-center justify-between p-2 bg-white rounded">
                            <span>{follower.name}</span>
                            <div className="flex items-center space-x-2">
                              {user.messagesEnabled.includes(followerId) ? (
                                <span className="text-green-600 text-sm flex items-center">
                                  <CheckCircle className="w-4 h-4 mr-1" />
                                  Can Message
                                </span>
                              ) : (
                                <button
                                  onClick={() => enableMessagesFromBuyer(followerId)}
                                  className="text-blue-600 hover:text-blue-800 text-sm flex items-center"
                                >
                                  <Share2 className="w-4 h-4 mr-1" />
                                  Enable Messaging
                                </button>
                              )}
                            </div>
                          </div>
                        );
                      })}
                    </div>
                  </div>
                )}
              </div>

              {/* Products Section */}
              <div className="bg-white rounded-xl shadow-lg p-6 mb-8">
                <div className="flex justify-between items-center mb-6">
                  <h3 className="text-xl font-bold text-gray-900 font-['Bloomin_Gflow']">
                    Your Products ({getSellerProducts().length})
                  </h3>
                  <button
                    onClick={() => setCurrentView("create-product")}
                    className="bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-lg font-medium"
                  >
                    Add New Product
                  </button>
                </div>

                {getSellerProducts().length === 0 ? (
                  <div className="text-center py-12">
                    <div className="text-6xl mb-4">👕</div>
                    <h3 className="text-xl font-semibold text-gray-900 mb-2 font-['Bloomin_Gflow']">
                      No products yet
                    </h3>
                    <p className="text-gray-600 mb-4">Add your first product to start selling on Online Gikomba</p>
                    <button
                      onClick={() => setCurrentView("create-product")}
                      className="bg-blue-600 hover:bg-blue-700 text-white font-medium py-2 px-6 rounded-lg"
                    >
                      Add Product
                    </button>
                  </div>
                ) : (
                  <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    {getSellerProducts().map((product) => (
                      <div key={product.id} className="border border-gray-200 rounded-lg overflow-hidden">
                        <div className="relative">
                          <img 
                            src={product.image} 
                            alt={product.name}
                            className="w-full h-48 object-cover"
                          />
                          <button
                            onClick={() => deleteProduct(product.id)}
                            className="absolute top-2 right-2 bg-red-500 text-white p-1 rounded-full hover:bg-red-600"
                          >
                            <Trash2 className="w-4 h-4" />
                          </button>
                        </div>
                        
                        <div className="p-4">
                          <h4 className="font-semibold text-gray-900 mb-2">{product.name}</h4>
                          <div className="flex items-center mb-1">
                            <span className="text-lg font-bold text-gray-900">
                              Ksh {(product.price * (1 - product.discount/100)).toLocaleString()}
                            </span>
                            {product.discount > 0 && (
                              <span className="text-sm text-gray-500 line-through ml-2">
                                Ksh {product.price.toLocaleString()}
                              </span>
                            )}
                          </div>
                          
                          <div className="flex items-center justify-between mt-2">
                            <span className={`px-2 py-1 rounded text-xs font-medium ${
                              product.inStock ? 'bg-green-100 text-green-800' : 'bg-red-100 text-red-800'
                            }`}>
                              {product.inStock ? 'In Stock' : 'Out of Stock'}
                            </span>
                            {product.discount > 0 && (
                              <span className="px-2 py-1 bg-red-100 text-red-800 rounded text-xs font-medium">
                                {product.discount}% OFF
                              </span>
                            )}
                          </div>
                          
                          <div className="mt-3 pt-3 border-t flex justify-between items-center">
                            <span className="text-sm text-gray-600">
                              Followers notified: {user.followers.length}
                            </span>
                            <button className="p-2 text-gray-600 hover:text-blue-600">
                              <Edit3 className="w-4 h-4" />
                            </button>
                          </div>
                        </div>
                      </div>
                    ))}
                  </div>
                )}
              </div>

              {/* Follow Requests */}
              {followRequests.filter(r => r.sellerId === user.id && r.status === "pending").length > 0 && (
                <div className="bg-white rounded-xl shadow-lg p-6">
                  <h3 className="text-xl font-bold text-gray-900 mb-4">
                    Follow Requests ({followRequests.filter(r => r.sellerId === user.id && r.status === "pending").length})
                  </h3>
                  <div className="space-y-4">
                    {followRequests
                      .filter(r => r.sellerId === user.id && r.status === "pending")
                      .map(request => {
                        const buyer = sellers.find(s => s.id === request.buyerId) || { name: `User ${request.buyerId}` };
                        return (
                          <div key={request.id} className="flex items-center justify-between p-4 border border-gray-200 rounded-lg">
                            <div>
                              <div className="font-medium">{buyer.name}</div>
                              <div className="text-sm text-gray-600 flex items-center">
                                <Calendar className="w-4 h-4 mr-1" />
                                {new Date(request.timestamp).toLocaleDateString()}
                              </div>
                            </div>
                            <div className="flex space-x-2">
                              <button
                                onClick={() => acceptFollowRequest(request.id)}
                                className="bg-green-600 hover:bg-green-700 text-white px-3 py-1 rounded text-sm"
                              >
                                Accept
                              </button>
                              <button className="bg-gray-600 hover:bg-gray-700 text-white px-3 py-1 rounded text-sm">
                                Decline
                              </button>
                            </div>
                          </div>
                        );
                      })}
                  </div>
                </div>
              )}
            </div>
          </section>
        )}

        {currentView === "create-product" && user && (
          <section className="py-12">
            <div className="max-w-4xl mx-auto px-4">
              <div className="bg-white rounded-xl shadow-lg p-8">
                <div className="text-center mb-8">
                  <div className="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-4">
                    <Upload className="w-8 h-8 text-green-600" />
                  </div>
                  <h2 className="text-3xl font-bold text-gray-900 font-['Bloomin_Gflow'] mb-2">
                    Add New Product
                  </h2>
                  <p className="text-gray-600">
                    Upload photos and details of the clothes you want to sell
                  </p>
                </div>

                <div className="space-y-6">
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Product Name *
                    </label>
                    <input
                      type="text"
                      value={newProduct.name}
                      onChange={(e) => setNewProduct({...newProduct, name: e.target.value})}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="e.g., Classic White T-Shirt"
                    />
                  </div>
                  
                  <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <div>
                      <label className="block text-sm font-medium text-gray-700 mb-2">
                        Price (Ksh) *
                      </label>
                      <input
                        type="number"
                        value={newProduct.price}
                        onChange={(e) => setNewProduct({...newProduct, price: e.target.value})}
                        className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="e.g., 2500"
                      />
                    </div>
                    
                    <div>
                      <label className="block text-sm font-medium text-gray-700 mb-2">
                        Discount (%)
                      </label>
                      <input
                        type="number"
                        min="0"
                        max="100"
                        value={newProduct.discount}
                        onChange={(e) => setNewProduct({...newProduct, discount: e.target.value})}
                        className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="e.g., 10"
                      />
                    </div>
                    
                    <div>
                      <label className="block text-sm font-medium text-gray-700 mb-2">
                        Category *
                      </label>
                      <select
                        value={newProduct.category}
                        onChange={(e) => setNewProduct({...newProduct, category: e.target.value})}
                        className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      >
                        <option value="Tops">Tops</option>
                        <option value="Bottoms">Bottoms</option>
                        <option value="Dresses">Dresses</option>
                        <option value="Outerwear">Outerwear</option>
                        <option value="Accessories">Accessories</option>
                        <option value="Shoes">Shoes</option>
                      </select>
                    </div>
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Product Photo *
                    </label>
                    <div className="border-2 border-dashed border-gray-300 rounded-lg p-8 text-center">
                      <Upload className="w-12 h-12 text-gray-400 mx-auto mb-4" />
                      <p className="text-gray-600 mb-2">Drag & drop your product photo here</p>
                      <p className="text-sm text-gray-500">or</p>
                      <button className="mt-2 px-4 py-2 bg-blue-600 text-white rounded-lg hover:bg-blue-700">
                        Browse Files
                      </button>
                      <p className="text-xs text-gray-500 mt-2">JPG, PNG up to 5MB</p>
                    </div>
                  </div>
                  
                  <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div>
                      <label className="block text-sm font-medium text-gray-700 mb-2">
                        Available Colors (comma separated)
                      </label>
                      <input
                        type="text"
                        value={newProduct.colors}
                        onChange={(e) => setNewProduct({...newProduct, colors: e.target.value})}
                        className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="e.g., White, Black, Gray"
                      />
                    </div>
                    
                    <div>
                      <label className="block text-sm font-medium text-gray-700 mb-2">
                        Available Sizes (comma separated)
                      </label>
                      <input
                        type="text"
                        value={newProduct.sizes}
                        onChange={(e) => setNewProduct({...newProduct, sizes: e.target.value})}
                        className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                        placeholder="e.g., S, M, L, XL"
                      />
                    </div>
                  </div>
                  
                  <div>
                    <label className="block text-sm font-medium text-gray-700 mb-2">
                      Description
                    </label>
                    <textarea
                      value={newProduct.description}
                      onChange={(e) => setNewProduct({...newProduct, description: e.target.value})}
                      rows={4}
                      className="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                      placeholder="Describe your product..."
                    />
                  </div>
                </div>

                <div className="mt-8 flex justify-center space-x-4">
                  <button
                    onClick={() => setCurrentView("seller-dashboard")}
                    className="px-6 py-3 border border-gray-300 text-gray-700 rounded-lg hover:bg-gray-50 font-medium"
                  >
                    Cancel
                  </button>
                  <button
                    onClick={handleCreateProduct}
                    disabled={!newProduct.name || !newProduct.price}
                    className="px-6 py-3 bg-green-600 text-white rounded-lg hover:bg-green-700 font-medium disabled:opacity-50 disabled:cursor-not-allowed"
                  >
                    Add Product
                  </button>
                </div>
              </div>
            </div>
          </section>
        )}
      </main>

      {/* Notifications Dropdown */}
      {notifications.length > 0 && (
        <div className="fixed top-20 right-4 z-50 w-80 max-h-96 overflow-y-auto bg-white rounded-lg shadow-xl">
          <div className="p-4 border-b">
            <h3 className="font-bold">Notifications</h3>
          </div>
          <div className="divide-y">
            {notifications.slice(0, 10).map(notification => (
              <div key={notification.id} className={`p-4 ${notification.read ? 'bg-gray-50' : 'bg-blue-50'}`}>
                <div className="flex items-start">
                  <div className={`w-8 h-8 rounded-full flex items-center justify-center mr-3 ${
                    notification.type === 'error' ? 'bg-red-100 text-red-600' :
                    notification.type === 'follow-accepted' ? 'bg-green-100 text-green-600' :
                    notification.type === 'new-product' ? 'bg-purple-100 text-purple-600' :
                    'bg-blue-100 text-blue-600'
                  }`}>
                    {notification.type === 'error' ? '!' : 
                     notification.type === 'follow-accepted' ? <CheckCircle className="w-4 h-4" /> :
                     notification.type === 'new-product' ? <Plus className="w-4 h-4" /> :
                     <Bell className="w-4 h-4" />}
                  </div>
                  <div className="flex-1">
                    <p className="text-sm">{notification.message}</p>
                    <p className="text-xs text-gray-500 mt-1">
                      {new Date(notification.timestamp).toLocaleTimeString([], { hour: '2-digit', minute: '2-digit' })}
                    </p>
                  </div>
                </div>
              </div>
            ))}
          </div>
          <div className="p-2 text-center">
            <button 
              onClick={() => setNotifications([])}
              className="text-blue-600 hover:text-blue-800 text-sm"
            >
              Clear all notifications
            </button>
          </div>
        </div>
      )}

      {/* Footer */}
      <footer className="bg-gray-800 text-white py-12">
        <div className="container mx-auto px-4">
          <div className="grid grid-cols-1 md:grid-cols-4 gap-8">
            <div>
              <div className="flex items-center space-x-2 mb-4">
                <div className="w-8 h-8 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full"></div>
                <span className="text-xl font-bold font-['Bloomin_Gflow'] tracking-wide">
                  Online Gikomba
                </span>
              </div>
              <p className="text-gray-400">
                Kenya's premier online marketplace for buying and selling clothes.
              </p>
              <div className="mt-4 flex items-center text-sm">
                <seasonalTheme.icon className="w-4 h-4 mr-2" />
                <span>{seasonalTheme.name} • {seasonalTheme.description}</span>
              </div>
            </div>
            
            <div>
              <h3 className="font-bold text-lg mb-4 font-['Bloomin_Gflow']">For Buyers</h3>
              <ul className="space-y-2 text-gray-400">
                <li><a href="#" className="hover:text-white">How to Buy</a></li>
                <li><a href="#" className="hover:text-white">Shipping Information</a></li>
                <li><a href="#" className="hover:text-white">Returns Policy</a></li>
                <li><a href="#" className="hover:text-white">Buyer Protection</a></li>
              </ul>
            </div>
            
            <div>
              <h3 className="font-bold text-lg mb-4 font-['Bloomin_Gflow']">For Sellers</h3>
              <ul className="space-y-2 text-gray-400">
                <li><a href="#" className="hover:text-white">How to Sell</a></li>
                <li><a href="#" className="hover:text-white">Seller Fees</a></li>
                <li><a href="#" className="hover:text-white">Payment Methods</a></li>
                <li><a href="#" className="hover:text-white">Seller Support</a></li>
              </ul>
            </div>
            
            <div>
              <h3 className="font-bold text-lg mb-4 font-['Bloomin_Gflow']">Contact</h3>
              <ul className="space-y-2 text-gray-400">
                <li>Email: support@onlinegikomba.co.ke</li>
                <li>Phone: +254 700 000 000</li>
                <li>Nairobi, Kenya</li>
                <li className="mt-2 flex items-center">
                  <Calendar className="w-4 h-4 mr-2" />
                  {new Date().toLocaleDateString('en-KE', { 
                    weekday: 'long', 
                    year: 'numeric', 
                    month: 'long', 
                    day: 'numeric' 
                  })}
                </li>
              </ul>
            </div>
          </div>
          
          <div className="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
            <p>&copy; 2026 Online Gikomba. All rights reserved.</p>
          </div>
        </div>
      </footer>

      {/* Cart Sidebar */}
      {cartCount > 0 && (
        <div className="fixed bottom-4 right-4 z-50">
          <div className="bg-white rounded-lg shadow-xl p-6 w-80 max-h-96 overflow-y-auto">
            <div className="flex justify-between items-center mb-4">
              <h3 className="font-bold text-lg font-['Bloomin_Gflow']">Your Cart ({cartCount})</h3>
              <button 
                onClick={() => setCartItems([])}
                className="text-gray-500 hover:text-gray-700"
              >
                <X className="w-5 h-5" />
              </button>
            </div>
            
            <div className="space-y-4 mb-6">
              {cartItems.map((item) => (
                <div key={item.id} className="flex items-center space-x-3">
                  <img 
                    src={item.image} 
                    alt={item.name}
                    className="w-12 h-12 object-cover rounded"
                  />
                  <div className="flex-1">
                    <p className="font-medium text-sm">{item.name}</p>
                    <p className="text-gray-600 text-sm">
                      Ksh {(item.price * (1 - (item.discount || 0) / 100)).toLocaleString()} × {item.quantity}
                    </p>
                    <p className="text-xs text-gray-500">{item.seller.name}</p>
                  </div>
                  <button 
                    onClick={() => setCartItems(prev => 
                      prev.filter(i => i.id !== item.id)
                    )}
                    className="text-gray-400 hover:text-red-500"
                  >
                    <X className="w-4 h-4" />
                  </button>
                </div>
              ))}
            </div>
            
            <div className="border-t pt-4">
              <div className="flex justify-between mb-4">
                <span className="font-medium">Total:</span>
                <span className="font-bold text-lg">Ksh {cartTotal.toLocaleString()}</span>
              </div>
              <button className="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 rounded-lg">
                Checkout
              </button>
            </div>
          </div>
        </div>
      )}
    </div>
  );
}
