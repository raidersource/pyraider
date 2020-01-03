# PyRaider

> Using PyRaider You can scan installed dependencies known security vulnerabilities. It uses publicly known exploits, vulnerabilities database.
                            
                                    
## Usage

[Documentation](https://pyraider.raidersource.com/#/)

### Install `pyraider` using pip

```commandline
pip install pyraider
```

### Once a `pyraider` you can run help command. It will show you the list commands and examples.

```commandline
pyraider -h
```

### You can use `pyraider -v` to check the version.

```commandline
pyraider -v
```

##  Scan Vulnerabilities against the dependencies
> Using PyRaider you can scan the vulnerable packages.

### To run basic scan you can use `pyraider go` command. It will automatically detects the installed packages and scans against it and shows the report.

```commandline
pyraider go
```

### If you want to scan you packages against `requirements.txt` file.

```commandline
pyraider check -f requirements.txt
```

### If you want to scan the packages in the same directory.

```commandline
pyraider check -f .
```

## Reports
> PyRaider currently supports `JSON` and `CSV` formats.

### To Export as a `JSON` file.

```commandline
pyraider check -f requirments.txt -e json result.json
```

### To Export as a `CSV` file.

```commandline
pyraider check -f requirments.txt -e csv result.csv
```


## Out of Date Pacakges
> Using PyRaider you can check the latest packages. Aginst installed packages.

```commandline
pyraider validate -f requirments.txt
```


## Auto Fix
> PyRaider also supports `auto fix` feature. Using this you can fix the vulnerable packages.

**Note:** To updating the packages might affect your application.

### Fix
> You can fix packages vulnerabilities individually.

```
pyraider fix
```

### Autofix
> You can also fix packages vulnerabilities at one shot.


## Docker container
> You can also run `pyraider` has a docker container.

### Build docker container image

```
docker build -t pyraider .
```

### Powered by

[RaiderSource](https://raidersource.com)