# Project 2
# repo-Team1
Arish Soomar,  Rahim Bardai,  Hlina Tessema,  Adam Banini

## Setup/Install

### Clone the Repository
```bash
git clone <repository-url>
cd repo-Team1
cd Project2
```

### Usage

#### Open the Election System:
```bash
cd ElectionSystem
```

#### Compile: 
```bash
javac -d target/classes -sourcepath src src/**/*.java 
```
or 

```bash
mvn -q clean compile 
```

#### Run:
```bash
java -cp target/classes main.Main                                                  
```

Note: Make sure your CSV files are in the current working directory or provide the full path when prompted.

When you run the application, you'll be prompted to:
1. Enter CSV file name(s) for ballot data (e.g., `test/plurality_test.csv`)  
    Must contain:  
        a. Election Type  
        b. Seats  
3. Enable or disable shuffle mode (for STV)  
4. Winners will print to screen  
5. Log files will output (for STV)   



#### Run JUnit Tests
```bash
mvn test
```
