# Postman API Test Collections

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Newman](https://img.shields.io/badge/Newman-CLI-green?style=for-the-badge)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🎯 Overview

Collection of Postman API test suites with automated execution using Newman CLI and GitHub Actions CI/CD integration.

## 📦 Collections Included

This repository contains **5 API test collections**:

1. **Assignment #1** - `Assignment #1.postman_collection.json`
2. **Assignment #2** - `Assignment #2.postman_collection.json`
3. **Assignment #3** - `Assignment #3.postman_collection.json`
4. **Assignment #4** - `Assignment #4.postman_collection.json`
5. **Assignment #5** - `Assignment #5.postman_collection.json`

## ✨ Features

- ✅ **Automated API Testing** - Pre-configured test scripts
- ✅ **Newman CLI Integration** - Run collections from command line
- ✅ **CI/CD Ready** - GitHub Actions workflows included
- ✅ **Test Assertions** - Request/response validation
- ✅ **Environment Support** - Configurable for different environments

## 🚀 How to Use

### **Option 1: Import into Postman**

1. Open Postman application
2. Click **Import**
3. Select any `.postman_collection.json` file
4. Click **Import**
5. Run the collection

### **Option 2: Run with Newman CLI**

**Prerequisites:**
- Node.js installed
- Newman installed: `npm install -g newman`

**Run a collection:**
```bash
# Run Assignment #1
newman run "Assignment #1.postman_collection.json"

# Run with HTML report
newman run "Assignment #1.postman_collection.json" -r html

# Run with environment file
newman run "Assignment #1.postman_collection.json" -e environment.json
```

### **Option 3: Automated CI/CD**

Collections automatically run via GitHub Actions on:
- Push to main branch
- Pull requests
- Manual trigger

## 📁 Project Structure
```
Postman/
│
├── .github/workflows/
│   ├── postman.yml          # Postman collection runner
│   └── test.yml             # Test automation workflow
│
├── Assignment #1.postman_collection.json
├── Assignment #2.postman_collection.json
├── Assignment #3.postman_collection.json
├── Assignment #4.postman_collection.json
├── Assignment #5.postman_collection.json
│
└── README.md
```

## 🔧 Tech Stack

- **Postman** - API testing tool
- **Newman** - Command-line collection runner
- **GitHub Actions** - CI/CD automation
- **Node.js** - Runtime for Newman

## 📊 CI/CD Workflow

The GitHub Actions workflows automatically:
1. Install Newman
2. Run all collections
3. Generate test reports
4. Upload artifacts
5. Notify on failures

## 🧪 Sample Test Output
```bash
newman

Assignment #1

→ GET Request Example
  GET https://api.example.com/users [200 OK, 1.2KB, 345ms]
  ✓  Status code is 200
  ✓  Response contains user data

┌─────────────────────────┬────────────┬───────────┐
│                         │   executed │    failed │
├─────────────────────────┼────────────┼───────────┤
│              iterations │          1 │         0 │
├─────────────────────────┼────────────┼───────────┤
│                requests │          5 │         0 │
├─────────────────────────┼────────────┼───────────┤
│            test-scripts │         10 │         0 │
├─────────────────────────┼────────────┼───────────┤
│      assertions │         15 │         0 │
└─────────────────────────┴────────────┴───────────┘
```

## 📝 Adding New Collections

1. Create/export collection from Postman
2. Save as `.postman_collection.json`
3. Add to repository
4. Update this README
5. Commit and push

## 🤝 Best Practices

- Write clear test descriptions
- Use environment variables for dynamic values
- Add pre-request scripts for setup
- Include comprehensive assertions
- Organize requests logically

## 📧 Contact

**Sumit Narang**
- LinkedIn: [linkedin.com/in/sumit-narang15](https://www.linkedin.com/in/sumit-narang15)
- GitHub: [@snnarangsumit](https://github.com/snnarangsumit)

## 📄 License

This project is available for reference and learning purposes.

---

⭐ **If you find these collections helpful, please give this repo a star!**
