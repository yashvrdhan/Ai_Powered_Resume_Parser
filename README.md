# AI-Powered Resume Parser and Ranking System

An intelligent web application that leverages Natural Language Processing (NLP) and machine learning techniques to analyze, parse, and rank resumes against job descriptions. Built with a React frontend and Flask backend, this system provides an intuitive interface for automated resume screening and candidate ranking. 

![Resume Parser Banner](./frontend/public/banner.png)

## 🌟 Key Features

### 📄 Document Processing

- Support for multiple file formats (PDF, DOCX)
- Smart text extraction and section identification
- Automatic contact information extraction
- Bulk resume processing capabilities

### 🤖 AI-Powered Analysis

- Intelligent skill extraction and categorization
- Context-aware skill matching
- Natural language understanding
- Semantic similarity analysis
- Machine learning based ranking algorithm

### 🎯 Advanced Ranking

- Customizable skill categorization (Required/Essential/Good to Have)
- Weighted scoring system
- Comprehensive candidate evaluation
- Detailed skill gap analysis

### 💫 Modern User Interface

- Intuitive drag-and-drop file upload
- Interactive skill categorization
- Real-time processing feedback
- Beautiful responsive design
- Light/Dark theme support
- Downloadable detailed reports

## 🚀 Tech Stack

### Frontend

- React 18
- Vite
- TailwindCSS
- Context API
- Axios

### Backend

- Python 3.8+
- Flask
- spaCy
- NLTK
- PyPDF2
- python-docx

## 🛠️ Installation

### Prerequisites

- Node.js 14+
- Python 3.8+
- pip
- npm or yarn

### Backend Setup

1. Navigate to backend directory:

```bash
cd backend
```

2. Create and activate virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
.\venv\Scripts\activate   # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Download NLTK data:

```bash
python -c "import nltk; nltk.download('punkt'); nltk.download('averaged_perceptron_tagger'); nltk.download('stopwords')"
```

### Frontend Setup

1. Navigate to frontend directory:

```bash
cd frontend
```

2. Install dependencies:

```bash
npm install
# or
yarn install
```

### Environment Setup

1. Backend (.env):

```env
FLASK_ENV=development
UPLOAD_FOLDER=static/uploads
MAX_CONTENT_LENGTH=16777216
```

2. Frontend (.env):

```env
VITE_API_URL=http://localhost:5000
```

## 🚀 Running the Application

1. Start the backend server:

```bash
cd backend
python app.py
```

2. Start the frontend development server:

```bash
cd frontend
npm run dev
```

3. Access the application at: `http://localhost:5173`

## 📂 Project Structure

```
resume_ranking_system/
├── frontend/                 # React frontend application
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React contexts
│   │   └── utils/          # Utility functions
│   └── public/             # Static assets
│
├── backend/                 # Flask backend application
│   ├── app.py              # Main Flask application
│   ├── modules/
│   │   ├── document_processor.py
│   │   ├── skill_extractor.py
│   │   ├── resume_ranker.py
│   │   └── utils.py
│   ├── static/
│   │   └── uploads/        # File upload directory
│   └── templates/          # Report templates
```

## 🔄 How It Works

1. **Document Upload & Processing**

   - User uploads resumes and job description
   - System extracts text and identifies sections
   - Contact information is automatically parsed

2. **Skill Analysis**

   - AI identifies technical skills and competencies
   - Skills are matched against known patterns
   - Context and relevance are considered

3. **Interactive Categorization**

   - User categorizes job requirements
   - Skills are weighted based on importance
   - System adapts ranking algorithm accordingly

4. **Ranking & Results**
   - Candidates are scored based on matches
   - Detailed analysis is generated
   - Results are presented in intuitive UI

## 🔒 Security Features

- Secure file handling
- Input validation
- Session-based processing
- File size limits
- Directory traversal prevention

## 🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## 📄 License

MIT License - See [LICENSE](./LICENSE) for details

## 👥 Team

- Yash vardhan Singh Parmar - ML/NLP Implementation
- [Kunal Waldia] - Backend Development
- [Divyansh Dhaundiyal] - Frontend Development & UI/UX
