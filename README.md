git clone git@github.com:USER/REPO.git
cd REPO
git checkout -b replace-fusi-url-to-stronahandlowa
git grep -n "https://www.fusi-m.com/"
git ls-files -z | xargs -0 sed -i 's|https://www.fusi-m.com/|stronahandlowa|g'
