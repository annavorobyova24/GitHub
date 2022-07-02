1. На локальном репозитории сделать ветки:
- git branch Postman
- git branch Jmeter
- git branch CheckLists
- git branch BugReports
- git branch SQL
- git branch Charles
- git branch MobileTesting
2. Запушить все ветки на внешний репозиторий git push -u --all
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта cat > bug_report.txt
4. Запушить структуру багрепорта на внешний репозиторий
git add .
git commit -m "add bug report"
git push
5. Вмержить ветку Bag Reports в Main
git checkout main
git merge BugReports -m "merge bug report" 
6. Запушить main на внешний репозиторий.
git add .
git commit -m "new merge"
git push
7. В ветке CheckLists набросать структуру чек листа.
git checkout CheckLists
cat > checklist.txt
8. Запушить структуру на внешний репозиторий
git add .
git commit -m "add checklist"
git push
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
compare & pull request
10. Синхронизировать Внешнюю и Локальную ветки Main 
git pull
