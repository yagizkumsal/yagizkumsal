Write-Host "";
Write-Host ""; 

Write-Host " ";
Write-Host -ForegroundColor Blue "
Write-Host -ForegroundColor Red "HELLO STUPİD HACK";
Write-Host "";


# Get threat detection information and select desired fields
$threats = Get-MpThreatDetection | Select-Object InitialDetectionTime, LastThreatStatusChangeTime, ProcessName, Resources

# Display the information in a grid view
$threats | Out-GridView -PassThru -Title 'Windows Security 000x16x3b'
