# Smart Nursery Assistant — Technology Stack

**Program:** IEEE WIE JS Mentorship Program 2026  
**Track:** AI & Programming  
**Status:** Proposed technology choices

## 1. Application Type

**Responsive Web Application**

The first version will be developed as a web application that can be accessed through a browser on different screen sizes.

## 2. Proposed Technologies

| Component | Proposed Technology | Purpose |
|---|---|---|
| Frontend | HTML, CSS, JavaScript | Build the application interface |
| Backend | Python with Flask | Handle application requests and connect system components |
| AI and Computer Vision | Python with suitable machine-learning libraries | Process images and assess supported plant categories |
| Model Framework | TensorFlow or PyTorch — to be evaluated | Train and run the selected AI model |
| Data Storage | Database — not selected yet | Store plant records, inspections, care actions, and recommendations |
| Image Storage | To be selected | Store submitted plant images |
| Version Control | Git and GitHub | Track project changes and maintain the repository |
| Development Environment | Local development environment | Build and test the application |

## 3. Data Sources

Public plant-image datasets will be investigated as potential sources for model development.

Kaggle is one possible source, but no dataset has been finally selected or validated yet.

Before selecting a dataset, the project will evaluate:
- Supported plant types and conditions.
- Label quality and consistency.
- Image quality and diversity.
- Dataset size and suitability.
- Licensing and permitted use.
- Whether the data supports the intended assessment tasks.

Local nursery images may be reserved for independent evaluation rather than used for training or tuning.

## 4. Rejected or Deferred Choices

### Native Android Application
Not selected for the first version. A responsive web application is preferred as the initial delivery format.

### IoT and Sensor Integration
Deferred to a future stage. The first version will not depend on sensors or physical devices to measure soil moisture or control watering.

### Fixed Database or Deployment Platform
No final choice has been made yet. These decisions will be based on project needs and technical evaluation.

### Final AI Model and Framework
No final model or framework has been selected. TensorFlow and PyTorch remain candidates until the available data and model requirements are evaluated.

## 5. Technology Selection Principle

Technology choices should support the project requirements, the available development time, and the ability to demonstrate a working first version. Unconfirmed tools and technologies must not be presented as already implemented.