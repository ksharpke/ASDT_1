curl -u "ksharpke" https://api.github.com/user/repos -d '{"name":"ASDT_1", "private":true}'
git clone https://github.com/ksharpke/ASDT_1.git
cd ASDT_1
git checkout -b feature/about_me
echo "# Hakkımda\n\n**Ad:** Adınız\n**Ülke:** Ülkeniz\n**IT İlgi Alanları:** IT ilgi alanlarınız\n**Tercih Edilen Programlama Dilleri:** Tercih ettiğiniz diller" > README.md
git add README.md
git commit -m "Kendim hakkında bilgi ekle"
git push origin feature/about_me
echo "Ödev 1 Tamamlandı" > REPORT.pdf
git add REPORT.pdf
git commit -m "Tamamlama onayını içeren REPORT.pdf dosyası eklendi"
git push origin main
curl -u "ksharpke" -X PUT -d '' https://api.github.com/repos/ksharpke/ASDT_1/collaborators/Slowiczek
