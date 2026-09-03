git checkout main


touch week2.md
git add week2.md
git commit -m "Create week2.md"

git checkout -b week2


echo "working 1" >> week2.md
git add week2.md
git commit -m "working 1"

echo "working 2" >> week2.md
git add week2.md
git commit -m "working 2"

echo "This is line 3" >> week2.md
git add week2.md
git commit -m "Add 1 text line"

git checkout main

git checkout -b week2b

git merge --no-ff week2 -m "Merge branch 'week2' into week2b"

git branch -d week2

git checkout main
git checkout -b wip
touch wip.txt
git add wip.txt
git commit -m "Add wip.txt"

git checkout main
git merge week2b

git branch --merged >> week2.md
git branch --no-merged >> week2.md
git add week2.md
git commit -m "Add branch filter output"

git branch -d week2b

git branch -m wip work-in-progress
git push -u origin work-in-progress

git checkout work-in-progress
echo "Some new work" >> wip.txt
git add wip.txt
git commit -m "Update wip.txt"
git push origin work-in-progress
git branch -vv

git checkout main
git checkout -b experiment

touch exp1.txt
git add exp1.txt
git commit -m "Add exp1"

touch exp2.txt
git add exp2.txt
git commit -m "Add exp2"

git checkout main
touch main1.txt
git add main1.txt
git commit -m "Add main1 file"

git checkout experiment
git rebase main

git checkout main
echo "Rebase đã nhấc toàn bộ các commit của nhánh experiment và gắn chồng lên commit mới nhất của nhánh main, tạo thành một lịch sử đường thẳng tuyến tính." >> week2.md
git add week2.md
git commit -m "Explain rebase"

git merge experiment

git push origin main

