# Data_ware_house_10AC_weak2


```markdown
# Traffic Data Warehousing with Airflow and dbt

This project aims to build a scalable data warehousing tech stack for storing and analyzing vehicle trajectory data collected by swarm drones and static roadside cameras. The tech stack consists of PostgreSQL as the data warehouse, Apache Airflow for workflow orchestration, and dbt (Data Build Tool) for data transformations.

## Project Overview

The primary objective of this project is to create a data pipeline that can efficiently handle large volumes of vehicle trajectory data from the pNEUMA dataset. The pNEUMA dataset contains naturalistic trajectories of half a million vehicles collected by drones in the congested downtown area of Athens, Greece.

## Tech Stack

- **PostgreSQL**: An open-source relational database management system used as the data warehouse to store raw and transformed data.
- **Apache Airflow**: A workflow management platform used to orchestrate and schedule the data pipeline tasks.
- **dbt (Data Build Tool)**: A data transformation tool that follows the ELT (Extract, Load, Transform) approach, enabling SQL-based transformations on the data loaded into the data warehouse.

## Project Structure

```
.
├── airflow
│   └── dags
│       └── data_pipeline.py
├── dbt
│   ├── models
│   │   └── *.sql
│   ├── data
│   ├── macros
│   └── tests
├── scripts
│   └── load_data.py
├── README.md
└── requirements.txt
```

- `airflow/dags/data_pipeline.py`: Contains the Airflow DAG (Directed Acyclic Graph) definition for orchestrating the data pipeline tasks.
- `dbt/models/`: Directory containing SQL files for dbt data models and transformations.
- `dbt/data/`: Directory for storing sample data used for testing and development.
- `dbt/macros/`: Directory for custom dbt macros.
- `dbt/tests/`: Directory for dbt tests to ensure data quality.
- `scripts/load_data.py`: Python script for loading the pNEUMA dataset into the PostgreSQL data warehouse.
- `README.md`: This file.
- `requirements.txt`: Python package dependencies for the project.

## Getting Started

1. Clone the repository: `git clone https://github.com/your-repo/traffic-data-warehousing.git`
2. Install Python dependencies: `pip install -r requirements.txt`
3. Set up PostgreSQL and create a database for the project.
4. Configure Airflow and dbt with the appropriate database connections.
5. Load the pNEUMA dataset into the PostgreSQL data warehouse using the `load_data.py` script.
6. Run the Airflow DAG to orchestrate the data pipeline tasks.
7. Use dbt to create and run data transformations on the raw data.

## Documentation

- [Airflow Documentation](https://airflow.apache.org/docs/)
- [dbt Documentation](https://docs.getdbt.com/)
- [PostgreSQL Documentation](https://www.postgresql.org/docs/)

## Contributing

Contributions are welcome! Please follow the [contributing guidelines](...) to contribute to this project.

## License

This project is licensed under the [MIT License](LICENSE).
```

