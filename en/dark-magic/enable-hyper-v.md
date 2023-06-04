# Enable Hyper-V

#### Windows 10 Home

1. Create a file: **hyper.txt**
2. Copy and paste the following code into **hyper.txt**:

{% code title="hyper.bat" %}
```batch
pushd "%~dp0"

dir /b %SystemRoot%\servicing\Packages\*Hyper-V*.mum >hyper-v.txt

for /f %%i in ('findstr /i . hyper-v.txt 2^>nul') do dism /online /norestart /add-package:"%SystemRoot%\servicing\Packages\%%i"

del hyper-v.txt

Dism /online /enable-feature /featurename:Microsoft-Hyper-V-All /LimitAccess /ALL
```
{% endcode %}

3. Rename the file to: **hyper.bat**
4. Execute the file **hyper.bat**
5. Go to **Apps and Features** -> **Programs and Features** and Hyper-V should be visible now.
