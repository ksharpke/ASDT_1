curl -u "ASDT_1" https://api.github.com/user/repos -d '{"kemal":"ASDT_1", "private":true}'
git clone https://github.com/ksharpke/ASDT_1.git
cd ASDT_1
git checkout -b feature/about_me
echo "# Hakkımda\n\n**Ad:** kemalemreözdemir\n**Ülke:** Turkey\n**python:**cybersecurıty\n**python.csharp:** turkısh.english.polish" > README.md
git add README.md
git commit -m "ı lıke to go gym"
git push origin feature/about_me
echo "Ödev 1 Tamamlandı" > REPORT.pdf
git add REPORT.pdf
git commit -m "Tamamlama onayını içeren REPORT.pdf dosyası eklendi"
git push origin main
curl -u "ksharpke" -X PUT -d '' https://api.github.com/repos/ksharpke/ASDT_1/collaborators/Slowiczek
