# RCAgent
RCAgent - your AI on-call engineer that never sleeps. From alert to RCA in minutes, not hours

## Folder Structure 
```
├── rcagent/                  
│   ├── __init__.py
│   ├── main.py               
│   ├── config/               
│   │   ├── __init__.py
│   │   └── settings.py
│   ├── integrations/         
│   │   ├── __init__.py
│   │   ├── opsgenie_client.py
│   │   ├── opensearch_client.py
│   │   ├── grafana_client.py
│   │   ├── newrelic_client.py
│   │   └── gitlab_client.py
│   ├── core/                 
│   │   ├── __init__.py
│   │   ├── alert_handler.py
│   │   ├── incident_analyzer.py
│   │   ├── correlation_engine.py
│   │   └── rca_generator.py
│   ├── db/                   # Database layer
│   │   ├── __init__.py
│   │   ├── connection.py     # DB connection / session management
│   │   ├── models.py         # ORM or schema models
│   │   └── migrations/       # Optional, for migration scripts
│   ├── utils/                
│   │   ├── __init__.py
│   │   ├── logger.py
│   │   ├── time_utils.py
│   │   └── data_parser.py
│   ├── agents/               
│   │   ├── __init__.py
│   │   ├── llm_agent.py
│   │   └── prompt_templates.py
│   └── api/                  
│       ├── __init__.py
│       ├── server.py
│       └── routes.py
│
├── tests/                    
│   ├── __init__.py
│   ├── test_alert_handler.py
│   ├── test_integrations.py
│   ├── test_rca_generator.py
│   └── test_db.py           # DB-related tests
│
├── scripts/                  
│   ├── run_local.sh
│   └── seed_data.py
│
├── requirements.txt          
├── .env.example              
├── .gitignore
├── pyproject.toml            
├── README.md
└── Makefile                  
```
