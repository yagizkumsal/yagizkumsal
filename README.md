Write-Host "";
Write-Host ""; 
Write-Host -ForegroundColor Red "$$\     $$\  $$$$$$\   $$$$$$\  $$$$$$\$$$$$$$$\       $$\   $$\ $$\   $$\ $$\      $$\  $$$$$$\   $$$$$$\  $$\       ";
Write-Host -ForegroundColor Red "\$$\   $$  |$$  __$$\ $$  __$$\ \_$$  _\____$$  |      $$ | $$  |$$ |  $$ |$$$\    $$$ |$$  __$$\ $$  __$$\ $$ |      ";
Write-Host -ForegroundColor Red " \$$\ $$  / $$ /  $$ |$$ /  \__|  $$ |     $$  /       $$ |$$  / $$ |  $$ |$$$$\  $$$$ |$$ /  \__|$$ /  $$ |$$ |      ";
Write-Host -ForegroundColor Red "  \$$$$  /  $$$$$$$$ |$$ |$$$$\   $$ |    $$  /        $$$$$  /  $$ |  $$ |$$\$$\$$ $$ |\$$$$$$\  $$$$$$$$ |$$ |      ";
Write-Host -ForegroundColor Red "   \$$  /   $$  __$$ |$$ |\_$$ |  $$ |   $$  /         $$  $$<   $$ |  $$ |$$ \$$$  $$ | \____$$\ $$  __$$ |$$ |      ";
Write-Host -ForegroundColor Red "    $$ |    $$ |  $$ |$$ |  $$ |  $$ |  $$  /          $$ |\$$\  $$ |  $$ |$$ |\$  /$$ |$$\   $$ |$$ |  $$ |$$ |      ";
Write-Host -ForegroundColor Red "    $$ |    $$ |  $$ |\$$$$$$  |$$$$$$\$$$$$$$$\       $$ | \$$\ \$$$$$$  |$$ | \_/ $$ |\$$$$$$  |$$ |  $$ |$$$$$$$$\ ";
Write-Host -ForegroundColor Red "    \__|    \__|  \__| \______/ \______\________|      \__|  \__| \______/ \__|     \__| \______/ \__|  \__|\________|";
Write-Host " ";
Write-Host -ForegroundColor Blue "   Made By  / KENNEEDY <3
Write-Host -ForegroundColor Red "HELLO STUPİD HACK";
Write-Host "";


# Get threat detection information and select desired fields
$threats = Get-MpThreatDetection | Select-Object InitialDetectionTime, LastThreatStatusChangeTime, ProcessName, Resources

# Display the information in a grid view
$threats | Out-GridView -PassThru -Title 'Windows Security 000x16x3b'
