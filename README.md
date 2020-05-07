<h1 align="center"><img src="https://user-images.githubusercontent.com/26521948/72658109-63a1d400-39e7-11ea-9667-c652586b4508.png" alt="Apache JMeter logo" /></h1>
<h4 align="center">SOFTWARE TESTING ENTHUSIAST</h4>
<br>


# SeleniumMobSFScan
Selenium and Mobile Security Framework (MobSF) Integration to make Continuous Static Analysis possible.

## How to install MobSF in Docker
```
$ docker pull opensecurity/mobile-security-framework-mobsf
$ docker run -it -p 8000:8000 opensecurity/mobile-security-framework-mobsf:latest

Then Open browser and navigate to http://localhost:8000/
```

## How to Run Mobile Static Analysis with Selenium
```
i.e Android Installer (.apk)
$ mvn clean test -Dtest=MobileStaticAnalysis -Durl="http://localhost:8000/" -Dpath="/home/okta/Downloads/" -DapkName="eribank.apk"
```

```
i.e iOS installer (.ipa)
$ mvn clean test -Dtest=MobileStaticAnalysis -Durl="http://localhost:8000/" -Dpath="/home/okta/Downloads/" -DapkName="EriBank.ipa"
```

## References
- https://github.com/MobSF/Mobile-Security-Framework-MobSF
- https://www.selenium.dev/
