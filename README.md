# Mr. Sina - Advanced Medical Imaging Analysis Platform

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)](https://nextjs.org/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104%2B-009688?logo=fastapi)](https://fastapi.tiangolo.com/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-EE4C2C?logo=pytorch)](https://pytorch.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

Mr. Sina is a comprehensive medical imaging analysis platform designed for psychiatric and neurological applications. The system provides advanced brain MRI processing capabilities with a focus on clinical decision support, featuring both frontend and backend components with AI-powered analysis.

## 🌟 Key Features

### 🧠 Brain MRI Processing
- **PyTorch-based Analysis**: Deep learning models for brain region analysis
- **3D Image Processing**: Support for DICOM and NIfTI formats
- **Volumetric Analysis**: Quantitative measurements of brain structures
- **Heatmap Generation**: Attention visualization for brain regions
- **Clinical Interpretation**: AI-driven clinical insights and recommendations

### 🔬 Advanced FreeSurfer Integration
- **Cortical Surface Reconstruction**: Detailed 3D brain surface modeling
- **Subcortical Segmentation**: Analysis of 133 brain structures
- **Cortical Thickness Measurement**: Regional thickness calculations
- **Volumetric Analysis**: Precise volume measurements for all structures
- **Longitudinal Tracking**: Comparison of brain changes over time

### 📊 Clinical Decision Support
- **Risk Assessment**: Automated risk scoring algorithms
- **Treatment Recommendations**: AI-driven treatment suggestions
- **GAF Prediction**: Global Assessment of Functioning score estimation
- **Symptom Trajectory**: Predictive modeling of symptom development
- **Optimization Models**: Treatment plan optimization algorithms

### 👥 Patient Management
- **Comprehensive Profiles**: Detailed patient information management
- **Clinical Scales**: Support for multiple psychiatric assessment tools
- **Medication Tracking**: Complete treatment history management
- **MR Image Management**: Organized medical imaging repository
- **Progress Tracking**: Longitudinal patient monitoring

## 🏗️ Technology Stack

### Frontend
- **Next.js 15**: React-based framework with App Router and Turbopack
- **TypeScript**: Type-safe JavaScript development
- **Tailwind CSS**: Utility-first CSS framework
- **Recharts**: Data visualization components
- **Leaflet**: Interactive map components

### Backend
- **Python Services**: FastAPI-based microservices
- **PyTorch**: Deep learning framework
- **FreeSurfer**: Advanced neuroimaging analysis tools
- **MONAI**: Medical imaging AI framework
- **Streamlit**: Clinical data management applications

### Database
- **PostgreSQL**: Primary data storage
- **Prisma**: Database ORM

## 📁 Project Structure

```
mr-sina/
├── src/                    # Next.js frontend application
│   ├── app/               # App router pages and API routes
│   ├── components/        # React components
│   └── lib/               # Utility functions and services
├── python_services/       # Python backend services
│   ├── brain_mri_processor.py  # Core MRI processing
│   ├── huggingface_brain_seg.py # Advanced brain segmentation
│   ├── freesurfer_processor.py  # FreeSurfer integration
│   ├── main.py            # FastAPI service endpoints
│   ├── clinical_app/      # Streamlit clinical applications
│   └── models/            # AI models
├── prisma/                # Database schema and migrations
├── Metinler/              # Documentation and guides
└── README.md              # This file
```

## 🚀 Installation

### Prerequisites
- Node.js 14+
- Python 3.8+
- PostgreSQL
- FreeSurfer (for advanced analysis features)

### Frontend Setup
```bash
cd mr-sina
npm install
npm run dev
```

### Backend Setup
```bash
cd python_services
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 main.py
```

## 🧪 Services Architecture

```
Frontend (Next.js) ↔ API Layer (Next.js API Routes) ↔ Python Services (FastAPI) ↔ FreeSurfer Tools
```

### Available Services
1. **Brain MRI Processing Service**: Core image analysis capabilities
2. **Clinical Applications**: Streamlit-based clinical data management
3. **FreeSurfer Analysis Service**: Advanced neuroimaging analysis

## 📖 Documentation

- [FreeSurfer Integration Guide](Metinler/FREESURFER_INTEGRATION_GUIDE.md)
- [Clinical Decision Support Enhancements](Metinler/CLINICAL_DECISION_SUPPORT_ENHANCEMENTS.md)
- [Project Enhancements Summary](Metinler/PROJECT_ENHANCEMENTS_SUMMARY.md)
- [Final Implementation Summary](Metinler/FINAL_IMPLEMENTATION_SUMMARY.md)

## 🏃 Development

### Running the Application
1. Start the Python services: `cd python_services && python3 main.py`
2. Start the frontend: `npm run dev`
3. Access the application at `http://localhost:3000` (or next available port)

### Running Clinical Applications
```bash
cd python_services/clinical_app
streamlit run klinik_app.py
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is part of the MR-SINA medical imaging system and is intended for clinical and research use.

## 🆘 Support

For technical support or questions, please refer to the documentation or contact the development team.