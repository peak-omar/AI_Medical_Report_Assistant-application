# AI Agents for Medical Diagnostics

![AI Medical Assistant Banner](https://github.com/MGJillaniMughal/AI_Medical_Report_Assistant/assets/banner.png)

A Python-based project designed to create specialized LLM-powered AI agents that analyze complex medical cases. This system integrates insights from various medical professionals to provide comprehensive assessments and personalized treatment recommendations, showcasing the transformative potential of AI in multidisciplinary medicine.

## Current Version Overview

In the current version, we have implemented three AI agents leveraging GPT-4o, each specializing in a distinct aspect of medical analysis. A medical report is analyzed by these agents simultaneously using threading, based on their specific areas of expertise. Each agent provides recommendations and diagnoses from their perspective. After all AI agents complete their analyses, the results are summarized and consolidated into a cohesive report by a large language model, identifying three potential health issues for the patient.

### AI Agents

#### 1. Cardiologist Agent
- **Focus**: Identify potential cardiac issues, such as arrhythmias or structural abnormalities, that might not be apparent in initial evaluations.
- **Recommendation**: Suggest cardiovascular testing or continuous monitoring if necessary. Provide management strategies if a cardiovascular issue is identified.

#### 2. Psychologist Agent
- **Focus**: Assess if the symptoms align with psychological conditions such as panic disorder, anxiety, or stress-related issues.
- **Recommendation**: Propose psychological interventions like therapy, stress management, or medications. Evaluate the effectiveness of current psychological management.

#### 3. Pulmonologist Agent
- **Focus**: Determine if respiratory conditions, such as asthma or breathing disorders, are causing symptoms like shortness of breath or dizziness.
- **Recommendation**: Suggest additional respiratory evaluations, such as lung function tests, or recommend breathing exercises if a respiratory issue is suspected.

## Features

- Multidisciplinary analysis powered by specialized AI agents.
- Threaded execution for simultaneous agent processing.
- Consolidated diagnosis report highlighting three potential health issues.
- User-friendly interface for medical report uploads and AI-assisted insights.

## Future Enhancements

In future iterations, the system aims to:

- Include additional AI agents for neurology, endocrinology, immunology, and other specialties.
- Utilize the [Assistant API from OpenAI](https://platform.openai.com/docs/assistants/overview) with `function calling` and `code interpreter` capabilities.
- Implement advanced parsing techniques for handling complex medical reports.
- Introduce patient progress tracking and follow-up recommendation systems.

## Getting Started

### Prerequisites

- Python 3.9+
- OpenAI API Key
- Libraries: `streamlit`, `dotenv`, `fpdf`, `docx`, `PyPDF2`, `langchain`

### Repository Structure

```plaintext
.
├── app.py                     # Main application file
|   main.py                    # For Backend only
├── Utils
│   ├── Agents.py              # Definitions of specialized AI agents
├── Medical Reports            # Contains synthetic medical reports
|   ├── Medical Rerort - Sarah Mitchell.txt
|   ├── Medical Rerort - David Thompson.txt
|   ├── Medical Rerort - Emily Carter.txt
|   ├── Medical Rerort - Michael Johnson - Panic Attack Disorder.txt     
├── Results                    # Stores the outputs of the agent system
├── apikey.env                 # Your OpenAI API key file
└── README.md                  # Project documentation
```

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MGJillaniMughal/AI_Medical_Report_Assistant.git
   cd AI_Medical_Report_Assistant
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add your OpenAI API key:
   Create a `.env` file in the root directory and add:
   ```plaintext
   OPENAI_API_KEY=your_openai_api_key_here
   ```

4. Run the application:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Launch the Streamlit app and upload a medical report in TXT, PDF, or DOCX format.
2. Receive insights and diagnoses from the Cardiologist, Psychologist, and Pulmonologist agents.
3. View a consolidated report from the multidisciplinary team.
4. Interact with AI specialists via the chat interface to ask follow-up questions.
5. Save and download the diagnosis report in TXT, PDF, or Word format.

## Contributing

We welcome contributions to improve this project! Please follow these steps:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature description"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any queries, feel free to reach out via:
- **GitHub Issues**: [Issues](https://github.com/MGJillaniMughal/AI_Medical_Report_Assistant/issues)
- **Email**: m.g.jillani123@gmail.com
