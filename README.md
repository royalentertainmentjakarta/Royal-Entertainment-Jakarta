<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Royal Entertainment - Jasa Hiburan Band Dangdut Profesional dengan pengalaman lebih dari 10 tahun. Siap membuat acara Anda menjadi lebih berkesan dan meriah.">
    <meta name="keywords" content="band dangdut, hiburan dangdut, jasa musik dangdut, wedding entertainment, dangdut profesional">
    <title>Royal Entertainment - Jasa Hiburan Band Dangdut Profesional</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #D4AF37; /* Gold */
            --primary-dark: #B8941F;
            --primary-light: #E6C966;
            --secondary: #000000; /* Black */
            --light: #FFFFFF; /* White */
            --gray: #777777;
            --light-gray: #f8f8f8;
            --section-padding: 100px 0;
            --border-radius: 8px;
            --transition: all 0.3s ease;
            --box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            font-size: 16px;
            color: var(--secondary);
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--light);
        }
        
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Playfair Display', serif;
            font-weight: 600;
            margin-bottom: 20px;
            color: var(--secondary);
        }
        
        h1 {
            font-size: 3.5rem;
        }
        
        h2 {
            font-size: 2.5rem;
        }
        
        h3 {
            font-size: 1.8rem;
        }
        
        a {
            text-decoration: none;
            color: var(--primary);
            transition: var(--transition);
        }
        
        a:hover {
            color: var(--primary-dark);
        }
        
        img {
            max-width: 100%;
            height: auto;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }
        
        .section-title h2 {
            display: inline-block;
            position: relative;
            padding-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 80px;
            height: 3px;
            background-color: var(--primary);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--primary);
            color: var(--light);
            border-radius: var(--border-radius);
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: var(--transition);
            border: 2px solid var(--primary);
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: transparent;
            color: var(--primary);
        }
        
        .btn-outline {
            background-color: transparent;
            color: var(--primary);
        }
        
        .btn-outline:hover {
            background-color: var(--primary);
            color: var(--light);
        }
        
        /* Header & Navigation */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background-color: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(10px);
            transition: var(--transition);
        }
        
        header.scrolled {
            background-color: rgba(0, 0, 0, 0.95);
            box-shadow: var(--box-shadow);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            display: flex;
            align-items: center;
            font-size: 24px;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
            font-family: 'Playfair Display', serif;
        }
        
        .logo i {
            margin-right: 10px;
            font-size: 28px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            color: var(--light);
            font-weight: 500;
            position: relative;
            transition: var(--transition);
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        nav ul li a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            background-color: var(--primary);
            bottom: -5px;
            left: 0;
            transition: var(--transition);
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        .mobile-menu {
            display: none;
            font-size: 24px;
            color: var(--light);
            cursor: pointer;
        }
        
        /* Admin Panel */
        .admin-panel {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1001;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
        
        .admin-btn {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: var(--primary);
            color: var(--light);
            border: none;
            font-size: 20px;
            cursor: pointer;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .admin-btn:hover {
            background-color: var(--primary-dark);
            transform: scale(1.1);
        }
        
        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--light);
            position: relative;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at center, transparent 0%, rgba(0, 0, 0, 0.4) 100%);
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 800px;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            color: var(--primary);
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
            animation: fadeInDown 1s ease;
        }
        
        .hero p {
            font-size: 1.3rem;
            margin-bottom: 30px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            animation: fadeInUp 1s ease;
        }
        
        .hero-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            animation: fadeInUp 1s ease 0.3s;
            animation-fill-mode: both;
        }
        
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* About Section */
        .about {
            padding: var(--section-padding);
            background-color: var(--light);
            position: relative;
        }
        
        .about::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1516280440614-37939bbacd81?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            opacity: 0.05;
            z-index: -1;
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .about-text p {
            margin-bottom: 20px;
            color: var(--gray);
        }
        
        .about-image {
            flex: 1;
            position: relative;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
        }
        
        .about-image img {
            display: block;
            transition: var(--transition);
        }
        
        .about-image:hover img {
            transform: scale(1.05);
        }
        
        .about-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(212, 175, 55, 0.2) 0%, rgba(0, 0, 0, 0.5) 100%);
            z-index: 1;
        }
        
        /* Artists Section */
        .artists {
            padding: var(--section-padding);
            background: linear-gradient(rgba(0, 0, 0, 0.85), rgba(0, 0, 0, 0.85)), url('https://images.unsplash.com/photo-1511379938547-c1f69419868d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: var(--light);
        }
        
        .artists-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
        }
        
        .artist-card {
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.6) 0%, rgba(0, 0, 0, 0.8) 100%);
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            border: 1px solid rgba(212, 175, 55, 0.2);
            height: 100%;
            display: flex;
            flex-direction: column;
            position: relative;
        }
        
        .artist-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            border-color: var(--primary);
        }
        
        .artist-image {
            height: 250px;
            overflow: hidden;
            position: relative;
        }
        
        .artist-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .artist-card:hover .artist-image img {
            transform: scale(1.1);
        }
        
        .artist-image::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 50%;
            background: linear-gradient(to top, rgba(0, 0, 0, 0.8) 0%, transparent 100%);
        }
        
        .edit-photo-btn, .edit-social-btn {
            position: absolute;
            background-color: rgba(0, 0, 0, 0.7);
            color: var(--light);
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 10;
            transition: var(--transition);
            opacity: 0;
        }
        
        .edit-photo-btn {
            top: 10px;
            right: 10px;
        }
        
        .edit-social-btn {
            top: 10px;
            left: 10px;
        }
        
        .artist-card:hover .edit-photo-btn,
        .artist-card:hover .edit-social-btn {
            opacity: 1;
        }
        
        .edit-photo-btn:hover,
        .edit-social-btn:hover {
            background-color: var(--primary);
        }
        
        .artist-info {
            padding: 25px;
            flex: 1;
            display: flex;
            flex-direction: column;
        }
        
        .artist-name {
            font-size: 1.5rem;
            margin-bottom: 5px;
            color: var(--primary);
        }
        
        .artist-field {
            display: inline-block;
            background-color: var(--primary);
            color: var(--light);
            font-size: 0.8rem;
            font-weight: 500;
            padding: 5px 12px;
            border-radius: 20px;
            margin-bottom: 15px;
        }
        
        .artist-description {
            color: rgba(255, 255, 255, 0.8);
            margin-bottom: 15px;
            flex: 1;
        }
        
        .artist-social {
            display: flex;
            gap: 10px;
            margin-top: auto;
        }
        
        .artist-social a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 35px;
            height: 35px;
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--light);
            border-radius: 50%;
            transition: var(--transition);
        }
        
        .artist-social a:hover {
            background-color: var(--primary);
            transform: translateY(-3px);
        }
        
        /* Services Section */
        .services {
            padding: var(--section-padding);
            background: linear-gradient(rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.9)), url('https://images.unsplash.com/photo-1470225620780-dba8ba36b745?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: var(--light);
        }
        
        .packages {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .package-card {
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.7) 0%, rgba(0, 0, 0, 0.9) 100%);
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            position: relative;
            border: 1px solid rgba(212, 175, 55, 0.3);
        }
        
        .package-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            border-color: var(--primary);
        }
        
        .package-header {
            padding: 30px 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .package-card.low .package-header {
            background: linear-gradient(135deg, rgba(76, 175, 80, 0.2) 0%, rgba(0, 0, 0, 0.5) 100%);
        }
        
        .package-card.medium .package-header {
            background: linear-gradient(135deg, rgba(255, 152, 0, 0.2) 0%, rgba(0, 0, 0, 0.5) 100%);
        }
        
        .package-card.high .package-header {
            background: linear-gradient(135deg, rgba(244, 67, 54, 0.2) 0%, rgba(0, 0, 0, 0.5) 100%);
        }
        
        .package-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary) 0%, var(--primary-light) 100%);
        }
        
        .package-header h3 {
            font-size: 2rem;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        .package-price {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        .package-year {
            font-size: 0.9rem;
            color: var(--primary-light);
            margin-top: 5px;
        }
        
        .package-body {
            padding: 30px 20px;
        }
        
        .package-details {
            margin-bottom: 25px;
        }
        
        .package-details h4 {
            font-size: 1.2rem;
            margin-bottom: 15px;
            color: var(--primary);
            display: flex;
            align-items: center;
        }
        
        .package-details h4 i {
            margin-right: 10px;
        }
        
        .package-details ul {
            list-style: none;
            margin-left: 30px;
        }
        
        .package-details ul li {
            margin-bottom: 10px;
            position: relative;
            padding-left: 20px;
        }
        
        .package-details ul li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--primary);
        }
        
        .package-footer {
            text-align: center;
            padding: 0 20px 30px;
        }
        
        /* Gallery Section */
        .gallery {
            padding: var(--section-padding);
            background-color: var(--light);
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            border-radius: var(--border-radius);
            overflow: hidden;
            height: 250px;
            position: relative;
            cursor: pointer;
            box-shadow: var(--box-shadow);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        .gallery-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.7));
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: var(--transition);
        }
        
        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }
        
        .gallery-overlay i {
            color: var(--primary);
            font-size: 30px;
        }
        
        .gallery-edit-btn {
            position: absolute;
            top: 10px;
            right: 10px;
            background-color: rgba(0, 0, 0, 0.7);
            color: var(--light);
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 10;
            transition: var(--transition);
            opacity: 0;
        }
        
        .gallery-item:hover .gallery-edit-btn {
            opacity: 1;
        }
        
        .gallery-edit-btn:hover {
            background-color: var(--primary);
        }
        
        /* Lightbox */
        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.9);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }
        
        .lightbox-content {
            max-width: 90%;
            max-height: 90%;
            position: relative;
        }
        
        .lightbox-content img {
            max-width: 100%;
            max-height: 90vh;
            border: 3px solid var(--primary);
            border-radius: var(--border-radius);
        }
        
        .lightbox-close {
            position: absolute;
            top: -40px;
            right: 0;
            color: var(--light);
            font-size: 30px;
            cursor: pointer;
            transition: var(--transition);
        }
        
        .lightbox-close:hover {
            color: var(--primary);
        }
        
        /* Image Upload Modal */
        .upload-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 3000;
            justify-content: center;
            align-items: center;
        }
        
        .upload-modal-content {
            background-color: var(--light);
            padding: 30px;
            border-radius: var(--border-radius);
            max-width: 500px;
            width: 90%;
            position: relative;
        }
        
        .upload-modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 24px;
            color: var(--gray);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .upload-modal-close:hover {
            color: var(--primary);
        }
        
        .upload-modal h3 {
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .upload-preview {
            width: 100%;
            height: 200px;
            border: 2px dashed var(--gray);
            border-radius: var(--border-radius);
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            overflow: hidden;
            background-color: var(--light-gray);
        }
        
        .upload-preview img {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }
        
        .upload-preview i {
            font-size: 48px;
            color: var(--gray);
        }
        
        .upload-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        
        .file-input-wrapper {
            position: relative;
            overflow: hidden;
            display: inline-block;
        }
        
        .file-input-wrapper input[type=file] {
            position: absolute;
            left: 0;
            top: 0;
            opacity: 0;
            cursor: pointer;
            width: 100%;
            height: 100%;
        }
        
        .file-input-label {
            display: block;
            padding: 10px 15px;
            background-color: var(--primary);
            color: var(--light);
            border-radius: var(--border-radius);
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
        }
        
        .file-input-label:hover {
            background-color: var(--primary-dark);
        }
        
        .upload-buttons {
            display: flex;
            gap: 10px;
            justify-content: flex-end;
        }
        
        .btn-cancel {
            background-color: var(--gray);
        }
        
        .btn-cancel:hover {
            background-color: transparent;
            color: var(--gray);
        }
        
        /* Artist Social Media Modal */
        .artist-social-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 3000;
            justify-content: center;
            align-items: center;
        }
        
        .artist-social-modal-content {
            background-color: var(--light);
            padding: 30px;
            border-radius: var(--border-radius);
            max-width: 500px;
            width: 90%;
            position: relative;
        }
        
        .artist-social-modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 24px;
            color: var(--gray);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .artist-social-modal-close:hover {
            color: var(--primary);
        }
        
        .artist-social-modal h3 {
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .artist-name-display {
            text-align: center;
            margin-bottom: 20px;
            padding: 10px;
            background-color: var(--light-gray);
            border-radius: var(--border-radius);
            color: var(--primary);
            font-weight: 600;
        }
        
        .artist-social-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        
        .artist-social-input-group {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .artist-social-input-group i {
            font-size: 20px;
            width: 30px;
            text-align: center;
            color: var(--primary);
        }
        
        .artist-social-input-group input {
            flex: 1;
            padding: 10px 15px;
            border: 1px solid rgba(0, 0, 0, 0.1);
            border-radius: var(--border-radius);
            font-family: 'Poppins', sans-serif;
            font-size: 1rem;
            transition: var(--transition);
        }
        
        .artist-social-input-group input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.2);
        }
        
        .artist-social-buttons {
            display: flex;
            gap: 10px;
            justify-content: flex-end;
            margin-top: 10px;
        }
        
        /* Social Media Modal */
        .social-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 3000;
            justify-content: center;
            align-items: center;
        }
        
        .social-modal-content {
            background-color: var(--light);
            padding: 30px;
            border-radius: var(--border-radius);
            max-width: 500px;
            width: 90%;
            position: relative;
        }
        
        .social-modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 24px;
            color: var(--gray);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .social-modal-close:hover {
            color: var(--primary);
        }
        
        .social-modal h3 {
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .social-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        
        .social-input-group {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .social-input-group i {
            font-size: 20px;
            width: 30px;
            text-align: center;
            color: var(--primary);
        }
        
        .social-input-group input {
            flex: 1;
            padding: 10px 15px;
            border: 1px solid rgba(0, 0, 0, 0.1);
            border-radius: var(--border-radius);
            font-family: 'Poppins', sans-serif;
            font-size: 1rem;
            transition: var(--transition);
        }
        
        .social-input-group input:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.2);
        }
        
        .social-buttons {
            display: flex;
            gap: 10px;
            justify-content: flex-end;
            margin-top: 10px;
        }
        
        /* Testimonials Section */
        .testimonials {
            padding: var(--section-padding);
            background: linear-gradient(rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)), url('https://images.unsplash.com/photo-1511671782779-c97d3d27a1d4?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: var(--light);
        }
        
        .testimonial-container {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }
        
        .testimonial {
            margin-bottom: 50px;
            display: none;
        }
        
        .testimonial.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .testimonial-text {
            font-size: 1.2rem;
            font-style: italic;
            margin-bottom: 20px;
            position: relative;
            padding: 0 30px;
            line-height: 1.8;
        }
        
        .testimonial-text::before {
            content: '"';
            font-size: 4rem;
            color: var(--primary);
            position: absolute;
            left: -20px;
            top: -20px;
        }
        
        .testimonial-text::after {
            content: '"';
            font-size: 4rem;
            color: var(--primary);
            position: absolute;
            right: -20px;
            bottom: -40px;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: var(--primary);
        }
        
        .testimonial-author span {
            display: block;
            font-weight: 400;
            color: var(--light);
            font-size: 0.9rem;
        }
        
        .testimonial-dots {
            display: flex;
            justify-content: center;
            gap: 10px;
        }
        
        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.3);
            cursor: pointer;
            transition: var(--transition);
        }
        
        .dot.active {
            background-color: var(--primary);
        }
        
        /* Contact Section */
        .contact {
            padding: var(--section-padding);
            background-color: var(--light);
            position: relative;
        }
        
        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1493225457124-a3eb161ffa5f?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            opacity: 0.05;
            z-index: -1;
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
        }
        
        .contact-info {
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.03) 0%, rgba(0, 0, 0, 0.07) 100%);
            padding: 40px;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            border: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .contact-info h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
        }
        
        .contact-item i {
            font-size: 20px;
            color: var(--primary);
            margin-right: 15px;
            margin-top: 5px;
            width: 30px;
            text-align: center;
        }
        
        .contact-form {
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.03) 0%, rgba(0, 0, 0, 0.07) 100%);
            padding: 40px;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            border: 1px solid rgba(212, 175, 55, 0.2);
        }
        
        .contact-form h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid rgba(0, 0, 0, 0.1);
            border-radius: var(--border-radius);
            font-family: 'Poppins', sans-serif;
            font-size: 1rem;
            transition: var(--transition);
            background-color: rgba(255, 255, 255, 0.8);
        }
        
        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.2);
        }
        
        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }
        
        .form-message {
            display: none;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: var(--border-radius);
            text-align: center;
        }
        
        .form-message.success {
            display: block;
            background-color: rgba(76, 175, 80, 0.1);
            color: #4CAF50;
            border: 1px solid rgba(76, 175, 80, 0.3);
        }
        
        .form-message.error {
            display: block;
            background-color: rgba(244, 67, 54, 0.1);
            color: #F44336;
            border: 1px solid rgba(244, 67, 54, 0.3);
        }
        
        /* Footer */
        footer {
            background-color: var(--secondary);
            color: var(--light);
            padding: 70px 0 20px;
            position: relative;
        }
        
        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--primary) 0%, var(--primary-light) 100%);
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }
        
        .footer-col h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: var(--primary);
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h3::after {
            content: '';
            position: absolute;
            width: 50px;
            height: 3px;
            background-color: var(--primary);
            bottom: 0;
            left: 0;
        }
        
        .footer-col p {
            margin-bottom: 20px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .footer-col ul {
            list-style: none;
        }
        
        .footer-col ul li {
            margin-bottom: 10px;
        }
        
        .footer-col ul li a {
            color: rgba(255, 255, 255, 0.7);
            transition: var(--transition);
        }
        
        .footer-col ul li a:hover {
            color: var(--primary);
            padding-left: 5px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--light);
            border-radius: 50%;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background-color: var(--primary);
            transform: translateY(-5px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.5);
            font-size: 0.9rem;
        }
        
        /* Responsive */
        @media (max-width: 992px) {
            h1 {
                font-size: 3rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .contact-container {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 768px) {
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: rgba(0, 0, 0, 0.95);
                flex-direction: column;
                padding: 20px;
                box-shadow: var(--box-shadow);
            }
            
            nav ul.show {
                display: flex;
            }
            
            nav ul li {
                margin: 10px 0;
            }
            
            .mobile-menu {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .hero-buttons {
                flex-direction: column;
                gap: 15px;
            }
            
            .packages {
                grid-template-columns: 1fr;
            }
            
            .artists-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
            
            .admin-panel {
                bottom: 10px;
                right: 10px;
            }
        }
        
        @media (max-width: 576px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .gallery-grid {
                grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            }
            
            .artists-grid {
                grid-template-columns: 1fr;
            }
            
            .upload-modal-content,
            .social-modal-content,
            .artist-social-modal-content {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">
                <i class="fas fa-crown"></i>
                Royal Entertainment
            </a>
            <nav>
                <ul id="navMenu">
                    <li><a href="#home">Beranda</a></li>
                    <li><a href="#about">Tentang Kami</a></li>
                    <li><a href="#artists">Artis</a></li>
                    <li><a href="#services">Paket Layanan</a></li>
                    <li><a href="#gallery">Galeri</a></li>
                    <li><a href="#testimonials">Testimoni</a></li>
                    <li><a href="#contact">Kontak</a></li>
                </ul>
            </nav>
            <div class="mobile-menu" id="mobileMenu">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>
    
    <!-- Admin Panel -->
    <div class="admin-panel">
        <button class="admin-btn" id="socialMediaBtn" title="Update Media Sosial">
            <i class="fab fa-instagram"></i>
        </button>
        <button class="admin-btn" id="editModeBtn" title="Mode Edit">
            <i class="fas fa-edit"></i>
        </button>
    </div>
    
    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Royal Entertainment</h1>
            <p>Hiburan Dangdut Premium untuk Acara Istimewa Anda</p>
            <div class="hero-buttons">
                <a href="#services" class="btn">Lihat Paket Kami</a>
                <a href="#contact" class="btn btn-outline">Hubungi Kami</a>
            </div>
        </div>
    </section>
    
    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <div class="section-title">
                <h2>Tentang Kami</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Pengalaman Lebih Dari 10 Tahun</h3>
                    <p>Royal Entertainment adalah penyedia jasa hiburan band dangdut premium yang telah berpengalaman lebih dari 10 tahun dalam menghibur berbagai acara eksklusif di seluruh Indonesia.</p>
                    <p>Dengan personel yang berkompeten dan peralatan canggih, kami siap membuat acara Anda menjadi lebih berkesan dan meriah dengan penampilan musik dangdut yang energik dan menghibur.</p>
                    <p>Kami menawarkan berbagai paket layanan yang dapat disesuaikan dengan kebutuhan dan anggaran Anda, mulai dari acara intimate hingga acara besar dengan produksi lengkap.</p>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1511671782779-c97d3d27a1d4?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80" alt="Band Dangdut Performance">
                </div>
            </div>
        </div>
    </section>
    
    <!-- Artists Section -->
    <section id="artists" class="artists">
        <div class="container">
            <div class="section-title">
                <h2>Artis Kami</h2>
            </div>
            <div class="artists-grid">
                <!-- Artist 1 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist1/400/300.jpg" alt="Rina Surya">
                        <button class="edit-photo-btn" data-type="artist" data-id="1">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="1" data-artist-name="Rina Surya">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Rina Surya</h3>
                        <span class="artist-field">Penyanyi Utama</span>
                        <p class="artist-description">Penyanyi dangdut dengan vokal powerful dan panggung yang energik. Berpengalaman lebih dari 8 tahun di industri musik dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 2 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist2/400/300.jpg" alt="Budi Pratama">
                        <button class="edit-photo-btn" data-type="artist" data-id="2">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="2" data-artist-name="Budi Pratama">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Budi Pratama</h3>
                        <span class="artist-field">Keyboardist</span>
                        <p class="artist-description">Master keyboard dengan kemampuan improvisasi yang luar biasa. Spesialis dalam musik dangdut modern dan koplo.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 3 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist3/400/300.jpg" alt="Siti Rahayu">
                        <button class="edit-photo-btn" data-type="artist" data-id="3">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="3" data-artist-name="Siti Rahayu">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Siti Rahayu</h3>
                        <span class="artist-field">Penyanyi Duet</span>
                        <p class="artist-description">Penyanyi dengan suara merdu dan kemampuan duet yang harmonis. Spesialis lagu-lagu dangdut romantis.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 4 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist4/400/300.jpg" alt="Ahmad Fauzi">
                        <button class="edit-photo-btn" data-type="artist" data-id="4">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="4" data-artist-name="Ahmad Fauzi">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Ahmad Fauzi</h3>
                        <span class="artist-field">Drummer</span>
                        <p class="artist-description">Drummer dengan ritme yang stabil dan energik. Mampu memainkan berbagai genre musik dengan fokus pada dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 5 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist5/400/300.jpg" alt="Maya Putri">
                        <button class="edit-photo-btn" data-type="artist" data-id="5">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="5" data-artist-name="Maya Putri">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Maya Putri</h3>
                        <span class="artist-field">Penari</span>
                        <p class="artist-description">Penari profesional dengan gerakan yang lincah dan enerjik. Spesialis dalam tari-tarian tradisional dan modern dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 6 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist6/400/300.jpg" alt="Eko Wijaya">
                        <button class="edit-photo-btn" data-type="artist" data-id="6">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="6" data-artist-name="Eko Wijaya">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Eko Wijaya</h3>
                        <span class="artist-field">Bassist</span>
                        <p class="artist-description">Bassis dengan groove yang kuat dan stabil. Berpengalaman dalam berbagai genre musik dengan spesialisasi dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 7 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist7/400/300.jpg" alt="Dewi Lestari">
                        <button class="edit-photo-btn" data-type="artist" data-id="7">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="7" data-artist-name="Dewi Lestari">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Dewi Lestari</h3>
                        <span class="artist-field">Penyanyi Utama</span>
                        <p class="artist-description">Penyanyi dengan vokal yang kuat dan range yang luas. Spesialis dalam lagu-lagu dangdut klasik dan modern.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 8 - Zapen dengan gambar baru -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://z-cdn-media.chatglm.cn/files/8802115f-b3a3-47a5-9167-aa1974fded26_WhatsApp%20Image%202025-09-06%20at%2001.18.29.jpeg?auth_key=1788638958-6dafbaf0dbbd4089b9e6e6a3c9b83a72-0-bc679e06e4d16b3e0e0d0c3a2e8b2735" alt="Zapen">
                        <button class="edit-photo-btn" data-type="artist" data-id="8">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="8" data-artist-name="Zapen">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Zapen</h3>
                        <span class="artist-field">Gitaris Melodi</span>
                        <p class="artist-description">Gitaris dengan teknik melodi yang memukau. Mampu memainkan berbagai gendingan dangdut dengan sempurna.</p>
                        <div class="artist-social">
                            <a href="https://www.instagram.com/zavendhafinramadhan?igsh=MXRuaTN5eDF1Y3Nicg==" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="https://www.youtube.com/@skstudio1994" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="https://web.facebook.com/zaven.ramadhan?rdid=298hbnkKoUJjT5YX&share_url=https%3A%2F%2Fweb.facebook.com%2Fshare%2F1N9XSEHrXz%2F%3F_rdc%3D1%26_rdr#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="https://www.tiktok.com/@zavenghumballa?_t=ZS-8zTudpOXWNT&_r=1" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 9 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist9/400/300.jpg" alt="Indah Permata">
                        <button class="edit-photo-btn" data-type="artist" data-id="9">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="9" data-artist-name="Indah Permata">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Indah Permata</h3>
                        <span class="artist-field">Penari</span>
                        <p class="artist-description">Penari dengan fleksibilitas tinggi dan gerakan yang ekspresif. Spesialis dalam tari-tarian dangdut kontemporer.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 10 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist10/400/300.jpg" alt="Fajar Nugroho">
                        <button class="edit-photo-btn" data-type="artist" data-id="10">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="10" data-artist-name="Fajar Nugroho">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Fajar Nugroho</h3>
                        <span class="artist-field">Pemain Suling</span>
                        <p class="artist-description">Maestro suling dengan alunan yang memukau. Spesialis dalam musik dangdut etnik dan tradisional.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 11 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist11/400/300.jpg" alt="Laila Sari">
                        <button class="edit-photo-btn" data-type="artist" data-id="11">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="11" data-artist-name="Laila Sari">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Laila Sari</h3>
                        <span class="artist-field">Penyanyi Duet</span>
                        <p class="artist-description">Penyanyi dengan suara yang khas dan kemampuan beradaptasi dengan berbagai genre musik dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 12 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist12/400/300.jpg" alt="Hendra Kusuma">
                        <button class="edit-photo-btn" data-type="artist" data-id="12">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="12" data-artist-name="Hendra Kusuma">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Hendra Kusuma</h3>
                        <span class="artist-field">Pemain Kendang</span>
                        <p class="artist-description">Pemain kendang dengan ritme yang khas dan energik. Mampu mengiringi berbagai jenis lagu dangdut.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 13 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist13/400/300.jpg" alt="Yuni Kartika">
                        <button class="edit-photo-btn" data-type="artist" data-id="13">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="13" data-artist-name="Yuni Kartika">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Yuni Kartika</h3>
                        <span class="artist-field">Penyanyi Utama</span>
                        <p class="artist-description">Penyanyi dengan panggung yang karismatik dan vokal yang powerful. Spesialis lagu-lagu dangdut populer.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 14 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist14/400/300.jpg" alt="Agus Santoso">
                        <button class="edit-photo-btn" data-type="artist" data-id="14">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="14" data-artist-name="Agus Santoso">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Agus Santoso</h3>
                        <span class="artist-field">Gitaris Akustik</span>
                        <p class="artist-description">Gitaris akustik dengan permainan fingerstyle yang halus. Spesialis dalam lagu-lagu dangdut akustik.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 15 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist15/400/300.jpg" alt="Ratna Dewi">
                        <button class="edit-photo-btn" data-type="artist" data-id="15">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="15" data-artist-name="Ratna Dewi">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Ratna Dewi</h3>
                        <span class="artist-field">Penari</span>
                        <p class="artist-description">Penari dengan gerakan yang elegan dan grak yang memukau. Spesialis dalam tari-tarian tradisional Jawa.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 16 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist16/400/300.jpg" alt="Tommy Wijaya">
                        <button class="edit-photo-btn" data-type="artist" data-id="16">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="16" data-artist-name="Tommy Wijaya">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Tommy Wijaya</h3>
                        <span class="artist-field">Pemain Tamborin</span>
                        <p class="artist-description">Pemain tamborin dengan ritme yang ceria dan energik. Memberikan warna khas dalam setiap penampilan.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 17 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist17/400/300.jpg" alt="Sarah Amalia">
                        <button class="edit-photo-btn" data-type="artist" data-id="17">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="17" data-artist-name="Sarah Amalia">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Sarah Amalia</h3>
                        <span class="artist-field">Penyanyi Duet</span>
                        <p class="artist-description">Penyanyi dengan suara yang lembut dan harmonis. Spesialis dalam lagu-lagu dangdut romantis dan melankolis.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 18 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist18/400/300.jpg" alt="Bagus Pratama">
                        <button class="edit-photo-btn" data-type="artist" data-id="18">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="18" data-artist-name="Bagus Pratama">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Bagus Pratama</h3>
                        <span class="artist-field">Sound Engineer</span>
                        <p class="artist-description">Sound engineer profesional dengan pengalaman lebih dari 10 tahun. Memastikan kualitas suara terbaik setiap pertunjukan.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 19 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist19/400/300.jpg" alt="Nina Kartika">
                        <button class="edit-photo-btn" data-type="artist" data-id="19">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="19" data-artist-name="Nina Kartika">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Nina Kartika</h3>
                        <span class="artist-field">Penyanyi Utama</span>
                        <p class="artist-description">Penyanyi dengan vokal yang unik dan stage presence yang kuat. Spesialis dalam lagu-lagu dangdut koplo.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-youtube-link"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Artist 20 -->
                <div class="artist-card">
                    <div class="artist-image">
                        <img src="https://picsum.photos/seed/artist20/400/300.jpg" alt="Dedi Mulyadi">
                        <button class="edit-photo-btn" data-type="artist" data-id="20">
                            <i class="fas fa-camera"></i>
                        </button>
                        <button class="edit-social-btn" data-artist-id="20" data-artist-name="Dedi Mulyadi">
                            <i class="fas fa-share-alt"></i>
                        </button>
                    </div>
                    <div class="artist-info">
                        <h3 class="artist-name">Dedi Mulyadi</h3>
                        <span class="artist-field">Stage Manager</span>
                        <p class="artist-description">Stage manager berpengalaman yang mengatur setiap detail pertunjukan. Memastikan acara berjalan lancar dan profesional.</p>
                        <div class="artist-social">
                            <a href="#" class="artist-instagram-link"><i class="fab fa-instagram"></i></a>
                            <a href="#" class="artist-linkedin-link"><i class="fab fa-linkedin-in"></i></a>
                            <a href="#" class="artist-facebook-link"><i class="fab fa-facebook-f"></i></a>
                            <a href="#" class="artist-tiktok-link"><i class="fab fa-tiktok"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Services Section -->
    <section id="services" class="services">
        <div class="container">
            <div class="section-title">
                <h2>Paket Layanan Kami</h2>
            </div>
            <div class="packages">
                <!-- Package Low -->
                <div class="package-card low">
                    <div class="package-header">
                        <h3>PAKET LOW</h3>
                        <div class="package-price">Rp 3.000.000 - Rp 4.000.000</div>
                        <div class="package-year">Harga Terupdate 2025</div>
                    </div>
                    <div class="package-body">
                        <div class="package-details">
                            <h4><i class="fas fa-users"></i> Man Power</h4>
                            <ul>
                                <li>3 personel band (keyboard, gendang, bass)</li>
                                <li>1 penyanyi utama (pria/wanita)</li>
                                <li>1 soundman</li>
                                <li>Total: 5 orang</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-sliders-h"></i> Equipment</h4>
                            <ul>
                                <li>1 set keyboard standar</li>
                                <li>1 set drum pad</li>
                                <li>1 unit bass gitar + amplifier kecil</li>
                                <li>2 unit microphone standar</li>
                                <li>1 unit mixer sederhana (8 channel)</li>
                                <li>2 unit speaker aktif 300 watt</li>
                                <li>Kabel-kabel standar</li>
                                <li>1 set lighting sederhana (2 lampu par)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-clock"></i> Durasi</h4>
                            <ul>
                                <li>2 jam performance</li>
                                <li>(1x45 menit main, 15 menit istirahat, 45 menit main)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-star"></i> Fasilitas</h4>
                            <ul>
                                <li>Repertoar lagu dangdut populer (30 lagu)</li>
                                <li>Tidak termasuk transport dan akomodasi</li>
                                <li>Tidak termasuk sound system untuk MC/pembawa acara</li>
                            </ul>
                        </div>
                    </div>
                    <div class="package-footer">
                        <a href="#contact" class="btn">Pesan Sekarang</a>
                    </div>
                </div>
                
                <!-- Package Medium -->
                <div class="package-card medium">
                    <div class="package-header">
                        <h3>PAKET MEDIUM</h3>
                        <div class="package-price">Rp 6.000.000 - Rp 9.000.000</div>
                        <div class="package-year">Harga Terupdate 2025</div>
                    </div>
                    <div class="package-body">
                        <div class="package-details">
                            <h4><i class="fas fa-users"></i> Man Power</h4>
                            <ul>
                                <li>5 personel band (keyboard, gendang, bass, gitar melodi, tamborin)</li>
                                <li>2 penyanyi (1 pria, 1 wanita)</li>
                                <li>1 soundman</li>
                                <li>1 teknisi lighting</li>
                                <li>Total: 9 orang</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-sliders-h"></i> Equipment</h4>
                            <ul>
                                <li>1 set keyboard berkualitas</li>
                                <li>1 set drum lengkap</li>
                                <li>1 unit bass gitar + amplifier</li>
                                <li>1 unit gitar melodi + amplifier</li>
                                <li>1 unit tamborin</li>
                                <li>4 unit microphone berkualitas</li>
                                <li>1 unit mixer digital (16 channel)</li>
                                <li>4 unit speaker aktif 500 watt</li>
                                <li>2 unit monitor speaker</li>
                                <li>Kabel-kabel berkualitas</li>
                                <li>1 set lighting standar (4 lampu par, 2 moving head, 1 laser)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-clock"></i> Durasi</h4>
                            <ul>
                                <li>3 jam performance</li>
                                <li>(2x60 menit main, 30 menit istirahat, 60 menit main)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-star"></i> Fasilitas</h4>
                            <ul>
                                <li>Repertoar lagu dangdut populer dan koplo (60 lagu)</li>
                                <li>Termasuk transport untuk radius 50 km</li>
                                <li>Sound system untuk MC/pembawa acara</li>
                                <li>Backdrop sederhana dengan nama band</li>
                            </ul>
                        </div>
                    </div>
                    <div class="package-footer">
                        <a href="#contact" class="btn">Pesan Sekarang</a>
                    </div>
                </div>
                
                <!-- Package High -->
                <div class="package-card high">
                    <div class="package-header">
                        <h3>PAKET HIGH</h3>
                        <div class="package-price">Rp 12.000.000 - Rp 18.000.000</div>
                        <div class="package-year">Harga Terupdate 2025</div>
                    </div>
                    <div class="package-body">
                        <div class="package-details">
                            <h4><i class="fas fa-users"></i> Man Power</h4>
                            <ul>
                                <li>7 personel band (keyboard, gendang, bass, gitar melodi, gitar akustik, suling, tamborin)</li>
                                <li>3 penyanyi (1 pria, 2 wanita)</li>
                                <li>2 penari</li>
                                <li>1 soundman profesional</li>
                                <li>2 teknisi lighting</li>
                                <li>1 stage manager</li>
                                <li>Total: 16 orang</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-sliders-h"></i> Equipment</h4>
                            <ul>
                                <li>2 set keyboard high-end</li>
                                <li>1 set drum lengkap berkualitas tinggi</li>
                                <li>1 unit bass gitar + amplifier premium</li>
                                <li>2 unit gitar (melodi & akustik) + amplifier premium</li>
                                <li>1 set alat musik tradisional (suling, kendang, dll)</li>
                                <li>6 unit microphone wireless premium</li>
                                <li>1 unit mixer digital profesional (24+ channel)</li>
                                <li>6 unit speaker aktif 1000 watt</li>
                                <li>4 unit monitor speaker</li>
                                <li>Sistem kabel berkualitas tinggi</li>
                                <li>1 set lighting profesional (8 lampu par, 4 moving head, 2 laser, fog machine)</li>
                                <li>1 unit LED screen 3x2 meter</li>
                                <li>1 set pyrotechnic (efek api)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-clock"></i> Durasi</h4>
                            <ul>
                                <li>4 jam performance</li>
                                <li>(3x60 menit main, 30 menit istirahat total, 60 menit main)</li>
                            </ul>
                        </div>
                        <div class="package-details">
                            <h4><i class="fas fa-star"></i> Fasilitas</h4>
                            <ul>
                                <li>Repertoar lengkap (100+ lagu) termasuk dangdut klasik, populer, koplo, dan request</li>
                                <li>Termasuk transport dan akomodasi untuk radius 100 km</li>
                                <li>Sound system lengkap untuk semua kebutuhan acara</li>
                                <li>Backdrop premium dengan custom design</li>
                                <li>Dokumentasi foto dan video sederhana</li>
                                <li>Makeup dan kostum untuk penampil</li>
                                <li>Sound check dan teknikal meeting sebelum acara</li>
                            </ul>
                        </div>
                    </div>
                    <div class="package-footer">
                        <a href="#contact" class="btn">Pesan Sekarang</a>
                    </div>
                </div>
            </div>
            
            <div class="section-title" style="margin-top: 70px;">
                <h2>Catatan Tambahan</h2>
            </div>
            <div style="max-width: 800px; margin: 0 auto; text-align: center;">
                <ul style="list-style: none; text-align: left; display: inline-block;">
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        Harga dapat berubah sewaktu-waktu tergantung pada jarak, tanggal, dan permintaan khusus
                    </li>
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        DP 50% dibayarkan saat booking dan pelunasan dilakukan H-7 sebelum acara
                    </li>
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        Pembatalan booking H-14 akan dikenakan biaya 25% dari total harga
                    </li>
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        Request lagu harus disampaikan minimal 2 minggu sebelum acara
                    </li>
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        Kostum dan tema penampilan dapat disesuaikan dengan permintaan klien
                    </li>
                    <li style="margin-bottom: 15px; position: relative; padding-left: 30px;">
                        <i class="fas fa-check-circle" style="position: absolute; left: 0; top: 2px; color: var(--primary);"></i>
                        Untuk acara di luar Jawa, akan ada tambahan biaya transport dan akomodasi
                    </li>
                </ul>
            </div>
        </div>
    </section>
    
    <!-- Gallery Section -->
    <section id="gallery" class="gallery">
        <div class="container">
            <div class="section-title">
                <h2>Galeri</h2>
            </div>
            <div class="gallery-grid">
                <!-- Gallery Item 1 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery1/500/500.jpg" alt="Performance 1">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="1">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 2 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery2/500/500.jpg" alt="Performance 2">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="2">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 3 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery3/500/500.jpg" alt="Performance 3">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="3">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 4 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery4/500/500.jpg" alt="Performance 4">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="4">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 5 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery5/500/500.jpg" alt="Performance 5">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="5">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 6 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery6/500/500.jpg" alt="Performance 6">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="6">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 7 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery7/500/500.jpg" alt="Performance 7">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="7">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 8 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery8/500/500.jpg" alt="Performance 8">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="8">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 9 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery9/500/500.jpg" alt="Performance 9">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="9">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 10 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery10/500/500.jpg" alt="Performance 10">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="10">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 11 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery11/500/500.jpg" alt="Performance 11">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="11">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
                
                <!-- Gallery Item 12 -->
                <div class="gallery-item">
                    <img src="https://picsum.photos/seed/gallery12/500/500.jpg" alt="Performance 12">
                    <div class="gallery-overlay">
                        <i class="fas fa-search-plus"></i>
                    </div>
                    <button class="gallery-edit-btn" data-type="gallery" data-id="12">
                        <i class="fas fa-camera"></i>
                    </button>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials Section -->
    <section id="testimonials" class="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>Testimoni Klien</h2>
            </div>
            <div class="testimonial-container">
                <!-- Testimonial 1 -->
                <div class="testimonial active">
                    <p class="testimonial-text">Royal Entertainment benar-benar membuat acara pernikahan kami menjadi berkesan! Penampilan energik dan lagu-lagu yang familiar membuat semua tamu ikut bergoyang. Highly recommended!</p>
                    <p class="testimonial-author">Budi & Siti <span>Pernikahan - Jakarta</span></p>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="testimonial">
                    <p class="testimonial-text">Kami menggunakan Paket High untuk acara ulang tahun perusahaan dan hasilnya luar biasa. Sound system yang jernih, lighting yang spektakuler, dan penampilan yang profesional. Terima kasih Royal Entertainment!</p>
                    <p class="testimonial-author">PT. Maju Bersama <span>Corporate Event - Surabaya</span></p>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="testimonial">
                    <p class="testimonial-text">Sangat puas dengan pelayanan Royal Entertainment. Tim yang ramah, koordinasi yang mudah, dan penampilan yang sesuai dengan ekspektasi. Acara gathering keluarga kami menjadi meriah dan berkesan.</p>
                    <p class="testimonial-author">Kel. Wijaya <span>Family Gathering - Bandung</span></p>
                </div>
                
                <!-- Testimonial 4 -->
                <div class="testimonial">
                    <p class="testimonial-text">Royal Entertainment membantu kami dalam acara promosi produk. Musik yang energik dan interaksi dengan penonton yang baik membuat acara kami sukses dan banyak dikunjungi.</p>
                    <p class="testimonial-author">CV. Sejahtera <span>Product Launching - Semarang</span></p>
                </div>
                
                <!-- Testimonial 5 -->
                <div class="testimonial">
                    <p class="testimonial-text">Kami sudah beberapa kali menggunakan jasa Royal Entertainment untuk berbagai acara dan selalu puas. Konsistensi kualitas penampilan dan profesionalisme tim membuat kami tidak ragu untuk merekomendasikan mereka.</p>
                    <p class="testimonial-author">Ibu Ani <span>Event Organizer - Yogyakarta</span></p>
                </div>
            </div>
            
            <div class="testimonial-dots">
                <span class="dot active" data-index="0"></span>
                <span class="dot" data-index="1"></span>
                <span class="dot" data-index="2"></span>
                <span class="dot" data-index="3"></span>
                <span class="dot" data-index="4"></span>
            </div>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h2>Hubungi Kami</h2>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Informasi Kontak</h3>
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <div>
                            <h4>Alamat</h4>
                            <p>Jl. Dangdut No. 123, Jakarta Selatan, DKI Jakarta 12345</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-phone-alt"></i>
                        <div>
                            <h4>Telepon</h4>
                            <p>+62 812-3456-7890</p>
                            <p>+62 821-9876-5432</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <div>
                            <h4>Email</h4>
                            <p>info@royalentertainment.com</p>
                            <p>booking@royalentertainment.com</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-clock"></i>
                        <div>
                            <h4>Jam Operasional</h4>
                            <p>Senin - Jumat: 09:00 - 18:00</p>
                            <p>Sabtu: 10:00 - 16:00</p>
                            <p>Minggu & Hari Libur: Tutup</p>
                        </div>
                    </div>
                    <div class="social-links">
                        <a href="#" class="instagram-link"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="youtube-link"><i class="fab fa-youtube"></i></a>
                        <a href="#" class="facebook-link"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="tiktok-link"><i class="fab fa-tiktok"></i></a>
                    </div>
                </div>
                
                <div class="contact-form">
                    <h3>Formulir Pemesanan</h3>
                    <div class="form-message" id="formMessage"></div>
                    <form id="contactForm">
                        <div class="form-group">
                            <input type="text" id="name" name="name" placeholder="Nama Lengkap" required>
                        </div>
                        <div class="form-group">
                            <input type="email" id="email" name="email" placeholder="Email" required>
                        </div>
                        <div class="form-group">
                            <input type="tel" id="phone" name="phone" placeholder="Nomor Telepon" required>
                        </div>
                        <div class="form-group">
                            <select id="package" name="package" required>
                                <option value="">Pilih Paket Layanan</option>
                                <option value="low">Paket Low</option>
                                <option value="medium">Paket Medium</option>
                                <option value="high">Paket High</option>
                                <option value="custom">Paket Custom</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <input type="date" id="date" name="date" required>
                        </div>
                        <div class="form-group">
                            <input type="text" id="location" name="location" placeholder="Lokasi Acara" required>
                        </div>
                        <div class="form-group">
                            <textarea id="message" name="message" placeholder="Pesan Tambahan"></textarea>
                        </div>
                        <button type="submit" class="btn">Kirim Pesan</button>
                    </form>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-col">
                    <h3>Tentang Kami</h3>
                    <p>Royal Entertainment adalah penyedia jasa hiburan band dangdut profesional dengan pengalaman lebih dari 10 tahun. Kami siap membuat acara Anda menjadi lebih berkesan dan meriah.</p>
                    <div class="social-links">
                        <a href="#" class="instagram-link"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="youtube-link"><i class="fab fa-youtube"></i></a>
                        <a href="#" class="facebook-link"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="tiktok-link"><i class="fab fa-tiktok"></i></a>
                    </div>
                </div>
                
                <div class="footer-col">
                    <h3>Link Cepat</h3>
                    <ul>
                        <li><a href="#home">Beranda</a></li>
                        <li><a href="#about">Tentang Kami</a></li>
                        <li><a href="#artists">Artis</a></li>
                        <li><a href="#services">Paket Layanan</a></li>
                        <li><a href="#gallery">Galeri</a></li>
                        <li><a href="#testimonials">Testimoni</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>Layanan Kami</h3>
                    <ul>
                        <li><a href="#">Paket Low</a></li>
                        <li><a href="#">Paket Medium</a></li>
                        <li><a href="#">Paket High</a></li>
                        <li><a href="#">Paket Custom</a></li>
                        <li><a href="#">Wedding Entertainment</a></li>
                        <li><a href="#">Corporate Event</a></li>
                        <li><a href="#">Private Party</a></li>
                    </ul>
                </div>
                
                <div class="footer-col">
                    <h3>Newsletter</h3>
                    <p>Dapatkan informasi terbaru tentang promo dan event kami.</p>
                    <form style="margin-top: 20px;">
                        <div style="display: flex; margin-bottom: 10px;">
                            <input type="email" placeholder="Email Anda" style="flex: 1; padding: 10px; border: none; border-radius: 4px 0 0 4px;">
                            <button type="submit" class="btn" style="border-radius: 0 4px 4px 0;">Subscribe</button>
                        </div>
                    </form>
                </div>
            </div>
            
            <div class="copyright">
                <p>© 2025 Royal Entertainment. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
    
    <!-- Lightbox -->
    <div class="lightbox" id="lightbox">
        <div class="lightbox-content">
            <span class="lightbox-close" id="lightboxClose">×</span>
            <img src="" alt="Gallery Image">
        </div>
    </div>
    
    <!-- Image Upload Modal -->
    <div class="upload-modal" id="uploadModal">
        <div class="upload-modal-content">
            <span class="upload-modal-close" id="uploadModalClose">×</span>
            <h3>Upload Gambar</h3>
            <div class="upload-preview" id="uploadPreview">
                <i class="fas fa-image"></i>
            </div>
            <div class="upload-form">
                <div class="file-input-wrapper">
                    <input type="file" id="fileInput" accept="image/*">
                    <label for="fileInput" class="file-input-label">Pilih Gambar</label>
                </div>
                <div class="upload-buttons">
                    <button class="btn btn-cancel" id="uploadCancel">Batal</button>
                    <button class="btn" id="uploadSave">Simpan</button>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Artist Social Media Modal -->
    <div class="artist-social-modal" id="artistSocialModal">
        <div class="artist-social-modal-content">
            <span class="artist-social-modal-close" id="artistSocialModalClose">×</span>
            <h3>Update Media Sosial Artis</h3>
            <div class="artist-name-display" id="artistNameDisplay">Nama Artis</div>
            <div class="artist-social-form">
                <div class="artist-social-input-group">
                    <i class="fab fa-instagram"></i>
                    <input type="text" id="artistInstagram" placeholder="Link Instagram">
                </div>
                <div class="artist-social-input-group">
                    <i class="fab fa-youtube"></i>
                    <input type="text" id="artistYoutube" placeholder="Link YouTube">
                </div>
                <div class="artist-social-input-group">
                    <i class="fab fa-facebook-f"></i>
                    <input type="text" id="artistFacebook" placeholder="Link Facebook">
                </div>
                <div class="artist-social-input-group">
                    <i class="fab fa-tiktok"></i>
                    <input type="text" id="artistTiktok" placeholder="Link TikTok">
                </div>
                <div class="artist-social-buttons">
                    <button class="btn btn-cancel" id="artistSocialCancel">Batal</button>
                    <button class="btn" id="artistSocialSave">Simpan</button>
                </div>
            </div>
        </div>
    </div>
    
    <!-- Social Media Modal -->
    <div class="social-modal" id="socialModal">
        <div class="social-modal-content">
            <span class="social-modal-close" id="socialModalClose">×</span>
            <h3>Update Media Sosial</h3>
            <div class="social-form">
                <div class="social-input-group">
                    <i class="fab fa-instagram"></i>
                    <input type="text" id="instagram" placeholder="Link Instagram">
                </div>
                <div class="social-input-group">
                    <i class="fab fa-youtube"></i>
                    <input type="text" id="youtube" placeholder="Link YouTube">
                </div>
                <div class="social-input-group">
                    <i class="fab fa-facebook-f"></i>
                    <input type="text" id="facebook" placeholder="Link Facebook">
                </div>
                <div class="social-input-group">
                    <i class="fab fa-tiktok"></i>
                    <input type="text" id="tiktok" placeholder="Link TikTok">
                </div>
                <div class="social-buttons">
                    <button class="btn btn-cancel" id="socialCancel">Batal</button>
                    <button class="btn" id="socialSave">Simpan</button>
                </div>
            </div>
        </div>
    </div>
    
    <script>
        // Mobile Menu Toggle
        const mobileMenu = document.getElementById('mobileMenu');
        const navMenu = document.getElementById('navMenu');
        
        mobileMenu.addEventListener('click', () => {
            navMenu.classList.toggle('show');
        });
        
        // Header Scroll Effect
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            header.classList.toggle('scrolled', window.scrollY > 50);
        });
        
        // Smooth Scrolling for Navigation Links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    window.scrollTo({
                        top: target.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    navMenu.classList.remove('show');
                }
            });
        });
        
        // Testimonial Slider
        const testimonials = document.querySelectorAll('.testimonial');
        const dots = document.querySelectorAll('.dot');
        let currentTestimonial = 0;
        
        function showTestimonial(index) {
            testimonials.forEach(testimonial => {
                testimonial.classList.remove('active');
            });
            
            dots.forEach(dot => {
                dot.classList.remove('active');
            });
            
            testimonials[index].classList.add('active');
            dots[index].classList.add('active');
        }
        
        dots.forEach((dot, index) => {
            dot.addEventListener('click', () => {
                currentTestimonial = index;
                showTestimonial(currentTestimonial);
            });
        });
        
        // Auto-rotate testimonials
        setInterval(() => {
            currentTestimonial = (currentTestimonial + 1) % testimonials.length;
            showTestimonial(currentTestimonial);
        }, 5000);
        
        // Gallery Lightbox
        const galleryItems = document.querySelectorAll('.gallery-item');
        const lightbox = document.getElementById('lightbox');
        const lightboxClose = document.getElementById('lightboxClose');
        const lightboxImg = lightbox.querySelector('img');
        
        galleryItems.forEach(item => {
            item.addEventListener('click', () => {
                const img = item.querySelector('img');
                lightboxImg.src = img.src;
                lightbox.style.display = 'flex';
            });
        });
        
        lightboxClose.addEventListener('click', () => {
            lightbox.style.display = 'none';
        });
        
        lightbox.addEventListener('click', (e) => {
            if (e.target === lightbox) {
                lightbox.style.display = 'none';
            }
        });
        
        // Upload Modal
        const uploadModal = document.getElementById('uploadModal');
        const uploadModalClose = document.getElementById('uploadModalClose');
        const uploadCancel = document.getElementById('uploadCancel');
        const uploadSave = document.getElementById('uploadSave');
        const fileInput = document.getElementById('fileInput');
        const uploadPreview = document.getElementById('uploadPreview');
        
        let currentEditType = '';
        let currentEditId = '';
        
        // Edit Photo Buttons
        const editPhotoBtns = document.querySelectorAll('.edit-photo-btn');
        editPhotoBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                currentEditType = btn.getAttribute('data-type');
                currentEditId = btn.getAttribute('data-id');
                uploadModal.style.display = 'flex';
            });
        });
        
        // Gallery Edit Buttons
        const galleryEditBtns = document.querySelectorAll('.gallery-edit-btn');
        galleryEditBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                currentEditType = btn.getAttribute('data-type');
                currentEditId = btn.getAttribute('data-id');
                uploadModal.style.display = 'flex';
            });
        });
        
        // File Input Change
        fileInput.addEventListener('change', (e) => {
            const file = e.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = (e) => {
                    uploadPreview.innerHTML = `<img src="${e.target.result}" alt="Preview">`;
                };
                reader.readAsDataURL(file);
            }
        });
        
        // Close Upload Modal
        uploadModalClose.addEventListener('click', () => {
            uploadModal.style.display = 'none';
            resetUploadModal();
        });
        
        uploadCancel.addEventListener('click', () => {
            uploadModal.style.display = 'none';
            resetUploadModal();
        });
        
        // Save Upload
        uploadSave.addEventListener('click', () => {
            // In a real application, you would save the image to a server
            // For this demo, we'll just show a success message
            alert(`Gambar untuk ${currentEditType} ${currentEditId} berhasil disimpan!`);
            uploadModal.style.display = 'none';
            resetUploadModal();
        });
        
        function resetUploadModal() {
            fileInput.value = '';
            uploadPreview.innerHTML = '<i class="fas fa-image"></i>';
        }
        
        // Artist Social Media Modal
        const artistSocialModal = document.getElementById('artistSocialModal');
        const artistSocialModalClose = document.getElementById('artistSocialModalClose');
        const artistSocialCancel = document.getElementById('artistSocialCancel');
        const artistSocialSave = document.getElementById('artistSocialSave');
        const artistNameDisplay = document.getElementById('artistNameDisplay');
        
        let currentArtistId = '';
        let currentArtistName = '';
        
        // Edit Social Buttons
        const editSocialBtns = document.querySelectorAll('.edit-social-btn');
        editSocialBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                currentArtistId = btn.getAttribute('data-artist-id');
                currentArtistName = btn.getAttribute('data-artist-name');
                
                // Display artist name
                artistNameDisplay.textContent = currentArtistName;
                
                // Get current social links
                const artistCard = btn.closest('.artist-card');
                const instagramLink = artistCard.querySelector('.artist-instagram-link').getAttribute('href');
                const youtubeLink = artistCard.querySelector('.artist-youtube-link').getAttribute('href');
                const facebookLink = artistCard.querySelector('.artist-facebook-link')?.getAttribute('href') || '';
                const tiktokLink = artistCard.querySelector('.artist-tiktok-link').getAttribute('href');
                
                // Fill form with current values
                document.getElementById('artistInstagram').value = instagramLink === '#' ? '' : instagramLink;
                document.getElementById('artistYoutube').value = youtubeLink === '#' ? '' : youtubeLink;
                document.getElementById('artistFacebook').value = facebookLink === '#' ? '' : facebookLink;
                document.getElementById('artistTiktok').value = tiktokLink === '#' ? '' : tiktokLink;
                
                artistSocialModal.style.display = 'flex';
            });
        });
        
        // Close Artist Social Modal
        artistSocialModalClose.addEventListener('click', () => {
            artistSocialModal.style.display = 'none';
        });
        
        artistSocialCancel.addEventListener('click', () => {
            artistSocialModal.style.display = 'none';
        });
        
        // Save Artist Social
        artistSocialSave.addEventListener('click', () => {
            // Get form values
            const instagramValue = document.getElementById('artistInstagram').value;
            const youtubeValue = document.getElementById('artistYoutube').value;
            const facebookValue = document.getElementById('artistFacebook').value;
            const tiktokValue = document.getElementById('artistTiktok').value;
            
            // Find the artist card
            const artistCards = document.querySelectorAll('.artist-card');
            artistCards.forEach(card => {
                const editBtn = card.querySelector(`.edit-social-btn[data-artist-id="${currentArtistId}"]`);
                if (editBtn) {
                    // Update social links
                    const instagramLink = card.querySelector('.artist-instagram-link');
                    const youtubeLink = card.querySelector('.artist-youtube-link');
                    const facebookLink = card.querySelector('.artist-facebook-link');
                    const tiktokLink = card.querySelector('.artist-tiktok-link');
                    
                    if (instagramValue) {
                        instagramLink.setAttribute('href', instagramValue);
                    } else {
                        instagramLink.setAttribute('href', '#');
                    }
                    
                    if (youtubeValue) {
                        youtubeLink.setAttribute('href', youtubeValue);
                    } else {
                        youtubeLink.setAttribute('href', '#');
                    }
                    
                    if (facebookLink && facebookValue) {
                        facebookLink.setAttribute('href', facebookValue);
                    } else if (facebookLink) {
                        facebookLink.setAttribute('href', '#');
                    }
                    
                    if (tiktokValue) {
                        tiktokLink.setAttribute('href', tiktokValue);
                    } else {
                        tiktokLink.setAttribute('href', '#');
                    }
                }
            });
            
            // Show success message
            alert(`Media sosial untuk ${currentArtistName} berhasil diperbarui!`);
            
            // Close modal
            artistSocialModal.style.display = 'none';
        });
        
        // Social Media Modal
        const socialModal = document.getElementById('socialModal');
        const socialModalClose = document.getElementById('socialModalClose');
        const socialCancel = document.getElementById('socialCancel');
        const socialSave = document.getElementById('socialSave');
        const socialMediaBtn = document.getElementById('socialMediaBtn');
        
        // Social Media Button
        socialMediaBtn.addEventListener('click', () => {
            // Get current social links
            const instagramLink = document.querySelector('.instagram-link').getAttribute('href');
            const youtubeLink = document.querySelector('.youtube-link').getAttribute('href');
            const facebookLink = document.querySelector('.facebook-link').getAttribute('href');
            const tiktokLink = document.querySelector('.tiktok-link').getAttribute('href');
            
            // Fill form with current values
            document.getElementById('instagram').value = instagramLink === '#' ? '' : instagramLink;
            document.getElementById('youtube').value = youtubeLink === '#' ? '' : youtubeLink;
            document.getElementById('facebook').value = facebookLink === '#' ? '' : facebookLink;
            document.getElementById('tiktok').value = tiktokLink === '#' ? '' : tiktokLink;
            
            socialModal.style.display = 'flex';
        });
        
        // Close Social Modal
        socialModalClose.addEventListener('click', () => {
            socialModal.style.display = 'none';
        });
        
        socialCancel.addEventListener('click', () => {
            socialModal.style.display = 'none';
        });
        
        // Save Social
        socialSave.addEventListener('click', () => {
            // Get form values
            const instagramValue = document.getElementById('instagram').value;
            const youtubeValue = document.getElementById('youtube').value;
            const facebookValue = document.getElementById('facebook').value;
            const tiktokValue = document.getElementById('tiktok').value;
            
            // Update social links
            const instagramLinks = document.querySelectorAll('.instagram-link');
            const youtubeLinks = document.querySelectorAll('.youtube-link');
            const facebookLinks = document.querySelectorAll('.facebook-link');
            const tiktokLinks = document.querySelectorAll('.tiktok-link');
            
            instagramLinks.forEach(link => {
                if (instagramValue) {
                    link.setAttribute('href', instagramValue);
                } else {
                    link.setAttribute('href', '#');
                }
            });
            
            youtubeLinks.forEach(link => {
                if (youtubeValue) {
                    link.setAttribute('href', youtubeValue);
                } else {
                    link.setAttribute('href', '#');
                }
            });
            
            facebookLinks.forEach(link => {
                if (facebookValue) {
                    link.setAttribute('href', facebookValue);
                } else {
                    link.setAttribute('href', '#');
                }
            });
            
            tiktokLinks.forEach(link => {
                if (tiktokValue) {
                    link.setAttribute('href', tiktokValue);
                } else {
                    link.setAttribute('href', '#');
                }
            });
            
            // Show success message
            alert('Media sosial berhasil diperbarui!');
            
            // Close modal
            socialModal.style.display = 'none';
        });
        
        // Edit Mode Toggle
        const editModeBtn = document.getElementById('editModeBtn');
        let editMode = false;
        
        editModeBtn.addEventListener('click', () => {
            editMode = !editMode;
            
            if (editMode) {
                editModeBtn.style.backgroundColor = '#4CAF50';
                editModeBtn.innerHTML = '<i class="fas fa-check"></i>';
                
                // Show all edit buttons
                document.querySelectorAll('.edit-photo-btn, .edit-social-btn, .gallery-edit-btn').forEach(btn => {
                    btn.style.opacity = '1';
                });
            } else {
                editModeBtn.style.backgroundColor = '';
                editModeBtn.innerHTML = '<i class="fas fa-edit"></i>';
                
                // Hide all edit buttons
                document.querySelectorAll('.edit-photo-btn, .edit-social-btn, .gallery-edit-btn').forEach(btn => {
                    btn.style.opacity = '';
                });
            }
        });
        
        // Contact Form
        const contactForm = document.getElementById('contactForm');
        const formMessage = document.getElementById('formMessage');
        
        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            // Get form values
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const phone = document.getElementById('phone').value;
            const package = document.getElementById('package').value;
            const date = document.getElementById('date').value;
            const location = document.getElementById('location').value;
            const message = document.getElementById('message').value;
            
            // Simple validation
            if (!name || !email || !phone || !package || !date || !location) {
                formMessage.className = 'form-message error';
                formMessage.textContent = 'Harap isi semua field yang wajib diisi!';
                return;
            }
            
            // In a real application, you would send this data to a server
            // For this demo, we'll just show a success message
            formMessage.className = 'form-message success';
            formMessage.textContent = 'Pesan Anda telah terkirim! Kami akan menghubungi Anda segera.';
            
            // Reset form
            contactForm.reset();
            
            // Hide message after 5 seconds
            setTimeout(() => {
                formMessage.className = 'form-message';
                formMessage.textContent = '';
            }, 5000);
        });
    </script>
</body>
</html>

