## Setup

### Requirements
- JDK 11
- Git
- Docker
- Docker Compose

### Load containers
#### Linux
```sh
git clone https://github.com/sourceplusplus/orbital
cd orbital
./gradlew composeUp && sleep 10 && ./setup-superset.sh
```

#### Windows
```sh
git clone https://github.com/sourceplusplus/orbital
cd orbital
gradlew.bat composeUp && timeout 10 && setup-superset.bat
```

### Available Services
- Apache Superset: http://167.99.134.5:8888
- Apache SkyWalking: http://167.99.134.5:9999

## Using Superset
- Add SkyWalking database to Superset
  - `postgresql+psycopg2://postgres:123456@postgres:5432/postgres`

## Using SkyWalking
- Click "Auto" in the top right corner if no charts displayed
- Change timezone in bottom right corner if no charts displayed
