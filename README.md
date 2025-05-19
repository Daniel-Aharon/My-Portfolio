# 🌐 Personal Portfolio Website

This is my personal portfolio website, built with **HTML**, **CSS**, and a bit of **JavaScript**, and hosted entirely on **AWS**. It serves as both a portfolio and a hands-on cloud project showcasing how to deploy a static website using modern cloud infrastructure.

## 🔗 Live Demo

👉 [https://danielaharon.site](https://danielaharon.site)

---

## 🛠 Tech Stack

- **Frontend**: HTML, CSS, JavaScript  
- **Hosting**: AWS S3 (static website hosting)  
- **Domain Management**: Route 53  
- **Security**: AWS Certificate Manager (SSL/TLS)  
- **CDN & HTTPS**: CloudFront  

---

## 🚀 Deployment Architecture

- **Amazon S3** – Stores the static site files (HTML, CSS, JavaScript, images, PDF)
- **Amazon Route 53** – Manages the custom domain: `danielaharon.site`
- **AWS Certificate Manager** – Provides an SSL certificate for HTTPS
- **Amazon CloudFront** – Distributes content securely and globally
- **HTTP ➝ HTTPS Redirect** – Configured through CloudFront to enforce secure traffic

---


## 📦 Deployment Steps (Manual)

1. **Upload files to S3**  
   Upload all website files (HTML, CSS, JavaScript, images, PDFs) to an S3 bucket with **static website hosting** enabled.

2. **Set bucket permissions**  
   Configure the bucket policy to allow **public read access** so users can view your site.

3. **Request an SSL certificate**  
   Use **AWS Certificate Manager (ACM)** to request a certificate for your custom domain (e.g., `danielaharon.site`).

4. **Create a CloudFront distribution**  
   Set up **CloudFront** to deliver content from your S3 bucket. Attach the SSL certificate and set your domain name as the alternate domain (CNAME).

5. **Connect domain with Route 53**  
   In **Amazon Route 53**, create an **A record (alias)** pointing your domain to the CloudFront distribution.

6. **Redirect HTTP to HTTPS**  
   In CloudFront’s behavior settings, configure a redirect from **HTTP to HTTPS** to ensure secure access.

## 📬 Contact

Feel free to reach out or connect with me:

- 🌐 Website: [https://danielaharon.site](https://danielaharon.site)
- 💼 LinkedIn: [https://www.linkedin.com/in/daniel-aharon5/](https://www.linkedin.com/in/daniel-aharon5/)
- 📧 Email: danielaharon53@gmail.com
