# Git for nerds 
- `git rebase`
- `git rebase --interactive`
- `git cherry-pick`
- `git reflog`

## Voraussetzungen
- Grundkenntnisse in Git (`git add`, `git commit`, ...)
- Tools:
  - [Git](https://git-scm.com/) (Ich verwende Version 2.39.5)
  - Texteditor (Ich benutze [Neovim](https://neovim.io/))
  - Remote Git-Repository (optional, [github](https://github.com/))
  - Repository-Visualisierungstool ([optional](https://github.com/git-up/GitUp))

## Rollen:
- X: Maintainerin oder Maintainer
- Y: Hilfsentwicklerin oder Hilfsentwickler

## A. Einfacher Rebase

1. - [x] X erstellt den ersten Commit in main
2. - [x] X macht eine kleine Änderung in einem zweiten Commit
3. - [x] Y erstellt einen Feature-Branch von main
4. - [x] Y macht Änderungen im Feature-Branch
5. - [x] X macht weitere Änderungen in main
6. - [ ] Y rebaset den Feature-Branch auf den aktuellen main

## B. Interaktiver Rebase (Squash und Umbenennen)

1. - [x] Y macht mehrere kleine Commits im Feature-Branch, die super wichtig sind, aber auch hart krass
2. - [ ] X beschwert sich über zu viele Commits, zu recht
3. - [ ] Y führt einen interaktiven Rebase durch, um:

## C. Cherry Pick

1. - [ ] Y erstellt einen experimentellen Branch
2. - [ ] Y macht einige Commits im experimentellen Branch
3. - [ ] X cherry-pickt einen spezifischen Commit in den main Branch

## D. Reflog

1. - [ ] Y macht versehentlich einen Rebase mit Drop eines wichtigen Commits
2. - [ ] Y nutzt reflog, um den verlorenen Zustand wiederherzustellen

## E. Wiederherstellung eines gelöschten Branches mit Reflog

1. - [ ] Y löscht versehentlich einen wichtigen Feature-Branch
2. - [ ] Mit Hilfe von reflog findet Y den letzten Commit des gelöschten Branches
3. - [ ] Ein neuer Branch wird basierend auf dem gefundenen Commit erstellt

## F. Abschluss und Fragen

1. - [ ] Zusammenfassung der wichtigsten Punkte
2. - [ ] Beantwortung von Fragen aus dem Publikum
