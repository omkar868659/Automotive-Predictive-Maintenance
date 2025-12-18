# Automotive Predictive Maintenance System

An AI-powered predictive maintenance system for vehicles using multi-agent architecture with LLM integration.

## Overview

This project implements an intelligent system that continuously analyzes vehicle telematics data and maintenance history to:
- Detect early warning signs of vehicle problems
- Forecast maintenance needs
- Generate service recommendations
- Optimize maintenance scheduling
- Communicate alerts to customers

## System Architecture

The system uses a multi-agent orchestration framework where specialized AI agents work together:

1. **Data Analysis Agent** - Analyzes streaming vehicle telematics and detects anomalies
2. **Diagnostic Agent** - Interprets data and generates detailed diagnostic reports
3. **Recommendation Agent** - Generates actionable maintenance recommendations
4. **Customer Engagement Agent** - AI voice calling and reporting
5. **Scheduling Agent** - Optimizes appointment scheduling and resource allocation
6. **Master Agent** - Handles all worker agents
7. **Manufacturing Quality Insights Module** - Provides insights and comprehensive reporting

## Key Features

- **Real-time Telematics Analysis** - Continuous streaming vehicle sensor data processing
- **Anomaly Detection** - Identifies abnormal sensor patterns and behaviors
- **Predictive Analytics** - Forecasts maintenance needs and service demand
- **Multi-agent Orchestration** - Coordinated workflow between specialized agents
- **LLM Integration** - Uses GPT models for intelligent analysis and reporting
- **Fleet Monitoring** - Tracks multiple vehicles simultaneously
- **Alert System** - Real-time notifications for critical issues

## Dependencies

- Python 3.8+
- pandas - Data manipulation and analysis
- numpy - Numerical computing
- matplotlib & seaborn - Data visualization
- langchain_openai - LLM integration
- langchain_core - LangChain core functionality
- langgraph - Agent orchestration framework

## Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/automotive-predictive-maintenance.git
cd automotive-predictive-maintenance
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Set up environment variables
```bash
export OPENAI_API_KEY="your-api-key-here"
```

4. Run the notebook
```bash
jupyter notebook "Automotive_Predictive_Maintainance_Code (1).ipynb"
```

## Data Files

The system requires the following CSV files:

- `vehicle_telemetry.csv` - Real-time sensor data from vehicles
- `maintainance_history_new - Sheet1.csv` - Historical maintenance records
- `Customer Database - Sheet2.csv` - Vehicle and customer information

## Usage

1. Start with Cell 1 to install dependencies
2. Run through the cells sequentially to:
   - Load and prepare data
   - Initialize the telematics API
   - Set up AI agents
   - Run the orchestration framework
   - Monitor and analyze results

## Project Structure

```
Predictve Maintenance code/
├── Automotive_Predictive_Maintainance_Code (1).ipynb  # Main notebook
├── vehicle_telemetry.csv                              # Telemetry data
├── maintainance_history_new - Sheet1.csv             # Maintenance history
├── Customer Database - Sheet2.csv                     # Customer data
├── README.md                                          # This file
└── .gitignore                                         # Git ignore rules
```

## API Configuration

Update the OpenAI API key in Cell 8:
```python
os.environ["OPENAI_API_KEY"] = "your-actual-api-key"
```

Or set it as an environment variable before running the notebook.

## Performance Metrics

The system evaluates performance based on:
- Prediction accuracy
- False positive rates
- Mean time to detection (MTTD)
- Resource utilization efficiency
- Cost savings from preventive maintenance

## Future Enhancements

- [ ] Integration with real vehicle OBD-II devices
- [ ] Predictive maintenance cost modeling
- [ ] Customer mobile app notifications
- [ ] Parts inventory optimization
- [ ] Technician scheduling integration
- [ ] Machine learning model refinement

## License

[Specify your license here]

**Note**: This system requires valid OpenAI API credentials to function. Ensure you have an active subscription with appropriate rate limits for production use.
