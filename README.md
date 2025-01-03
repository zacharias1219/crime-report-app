# **Crime Reporting Application - Safe Report**

This project introduces **Safe Report**, an innovative application allowing users to report crimes and incidents anonymously. Built using **Next.js 14**, **Gemini AI**, **Shadcn**, and **TailwindCSS**, the application combines modern frameworks and AI technology to ensure user anonymity, seamless reporting, and actionable administrative workflows.

---

## **Features**

- **Anonymous Reporting**:
  - Users can submit crime reports anonymously.
  - Two urgency levels: Emergency and Non-Emergency.
  
- **AI-Powered Analysis**:
  - Automatically identifies incident type and generates a detailed description using Gemini AI.
  - Generates unique report IDs for tracking purposes.

- **Interactive Admin Dashboard**:
  - Allows emergency authorities to review and manage reports.
  - Secured access via sign-in and sign-up systems.

- **Seamless UI Design**:
  - Built with Shadcn and TailwindCSS for a modern, user-friendly interface.

---

## **Tech Stack**

- **Frontend**: Next.js 14, Shadcn, TailwindCSS
- **Backend**: Prisma ORM, FastAPI
- **AI Integration**: Gemini AI for image analysis and automatic report generation
- **Database**: PostgreSQL
- **Utilities**: Mapbox for geolocation and auto-address filling

---

## **Setup and Installation**

### **Prerequisites**

- Node.js v16+
- PostgreSQL database
- API keys for Gemini AI and Mapbox

### **Installation Steps**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/safe-report.git
   cd safe-report
   ```

2. **Install Dependencies**:

   ```bash
   npm install
   ```

3. **Setup Environment Variables**:
   - Create a `.env` file in the root directory and include the following:

     ```env
     NEXT_PUBLIC_MAPBOX_ACCESS_TOKEN=your_mapbox_access_token
     GEMINI_AI_API_KEY=your_gemini_ai_api_key
     DATABASE_URL=your_postgres_database_url
     ```

4. **Set Up Prisma**:
   - Generate the Prisma client:

     ```bash
     npx prisma generate
     ```

   - Migrate the database schema:

     ```bash
     npx prisma migrate dev
     ```

5. **Run the Application**:

   ```bash
   npm run dev
   ```

   Access the application at `http://localhost:3000`.

---

## **Directory Structure**

```bash
├── app
│   ├── components
│   ├── pages
│   ├── services
│   ├── styles
│   └── utils
├── prisma
│   └── schema.prisma
├── public
│   └── assets
├── .env
├── README.md
└── package.json
```

---

## **Workflow Overview**

1. **Anonymous Reporting**:
   - Users upload images and provide location details.
   - AI generates report details based on uploaded images.

2. **Admin Dashboard**:
   - Review reports, update statuses, and manage submissions.

3. **Tracking Reports**:
   - Users track report statuses using unique IDs.

4. **Security Features**:
   - Authentication for admin access.
   - Data encryption for privacy protection.

---

## **Future Enhancements**

- Add multilingual support.
- Integrate SMS or email notifications for report updates.
- Expand AI capabilities for more detailed image analysis.

---

## **Contributing**

Contributions are welcome! Feel free to fork the repository, make enhancements, and submit a pull request.

---

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for details.

---
