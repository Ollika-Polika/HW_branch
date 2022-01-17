# HW_branch
HW 2.2 GitHub (Branch)

1. На локальном репозитории сделать ветки для:
- Postman /git branch Postman
- Jmeter /git branch Jmeter
- CheckLists /git branch CheckLists
- Bug Reports /git branch BugReports
- SQL /git branch SQL
- Charles /git branch Charles
- Mobile testing /git branch MobileTesting

2. Запушить все ветки на внешний репозиторий
/git push -u origin --all
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
git checkout BugReports
touch BugReport.txt
vim BugReport.txt
Bug report info
        id: 1,
        title: "Chat - User cannot rename group conversation"
        Type:  Bug,
        Priority: Medium,
        Affects Version: None,
        Component: None,
        Labels: None,
        Sprint: S22,
 Description
        Steps to reproduce
                  1) Log in,
                  2) Open chat dialog,
                  3) Click on the Setting button,
                  4) Add user,
                  5) Add user to a group conversation,
                  6) Try to rename this group conversation
        Expected result: User can rename group conversation.
        Actual result: Rename conversation button is disabled.
4. Запушить структуру багрепорта на внешний репозиторий
git add BugReport.txt
git commit -m "add BugReport.txt to repository"
git push
5. Вмержить ветку Bug Reports в Main
git checkout main
git merge BugReports
6. Запушить main на внешний репозиторий.
git push -u origin main
7. В ветке CheckLists набросать структуру чек листа.
git checkout CheckLists
cat > CheckList.txt
1 Login page
2 Add Company location
3 Add HR
4 Add user
5 Add user information
6 Edit user information
7 Delete user
8 Delete HR
9 Delete Company
8. Запушить структуру на внешний репозиторий
git add .
git commit -m "add Checklist.txt to repo"
git push
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
Ollika-Polika/HW_branch > Pull requests > Add pull request from CheckLists to main > Confirm
10. Синхронизировать Внешнюю и Локальную ветки Main
git pull
