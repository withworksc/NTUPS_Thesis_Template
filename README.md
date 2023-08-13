# 臺大政治系（非官方）碩士論文模板

## Summary
這個模板根據[Hsins](https://github.com/Hsins)大的[NTU-Thesis-LaTeX-Template](https://github.com/Hsins/NTU-Thesis-LaTeX-Template)所修改而來，並供臺大政治系研究生利用 [$\LaTeX$](https://www.latex-project.org) 撰寫論文。這個版本的模板大致上仍為持Hsins大所設計架構，並只有在以下幾處進行格式上的調整來更符合政治系的論文格式：

1. 引用格式：使用APA-6th，並從原本的Natbib套件改用Biblatex套件。
2. 目錄格式：對齊章節目錄的Chapter與Section標題。
3. 預設中文字體：主文預設字體由標楷體改變為思源宋體（新細明體有版權限制，故不上傳至Github，若要使用可以再自行更改）；圖、表標題與腳註則維持標楷體。
4. 口試委員審定書：修改為插入PDF頁面功能。
5. 調整所有目錄、章標題高度。

移除功能與設定：

1. 刪除在影印時預留的空白頁以及右側頁面開始章節的設定（twoside, openright）。
2. 刪除原有fonset功能，統一字型設定。
3. 刪除部分原有字體檔。

目前我大致只想到我有更改上述項目，畢竟這個模板是我在寫論文時邊寫邊改，有些修改的項目我可能忘記列上去。如果大家發現也提醒我一下。

## Notes

* 如果你需要新增字型，需先將字型檔加入`/fonts/-*`資料夾（或你可以放在專案資料夾任意處，as long as你知道你在做什麼），接著到`ntuthesis.cls`設定路徑與粗/斜體參數。
* 目前引用以及書目的標點符號仍為半型，全型的部分我還在想要怎麼解決。但目前版本已經過得了圖書館了，所以好像也不用太擔心（？
* 與前述類似，目前書目格式是APA-6th，不會隨著是中文或英文書目而改變書目格式。舉例來說，就是英文是APA、中文也會是APA，不會英文是APA但中文變政治科學論叢。同樣的，目前版本已經過得了圖書館，一樣不用太擔心（？
* 前面提到的問題我有空的時候可能會想辦法解決。使用的同學若想到解決方式或許也可以開個pull request。

## $\LaTeX$ Wiki

 * 不熟悉 $\LaTeX$ 操作的同學，你或許可以參考[sppmg](https://github.com/sppmg)大的[教學](https://github.com/sppmg/TW_Thesis_Template)。
 * 或者是[Overleaf的LaTeX教學](https://www.overleaf.com/learn/latex/Tutorials)。

## Structures

```
├── back
│   ├── appendix-*.tex              // 附錄
│   ├── references.bib              // 參考文獻
│   └── ...
├── contents
│   ├── chapter-*.tex               // 論文內容
│   ├── figures                     // 論文主文圖片資料夾
│   │     └── ... 
│   ├── tables                      // 論文主文表格資料夾
│   │     └── ...         
│   └── ...
├── figures
│   └── ...
├── fonts
│   ├── chinese
│   │   ├── BiauKai.ttf             // 標楷體
│   │   ├── NotoSansTC-*.otf        // 思源黑體
│   │   ├── SourceHanSerifTC-*.otf  // 思源宋體
│   │   └── ...
│   └── english
│       ├── Times New Roman-*.ttf   // Times New Roman 字體
│       ├── texgyrepagella-math.otf // Tex Gyre Pagella 數學字體
│       └── ...
├── front
│   ├── abstract.tex                // 摘要
│   ├── acknowledgement.tex         // 致謝
│   └── verification.tex            // 你的審定書（請記得覆蓋成系辦給你的版本）
├── main.tex                        // 主文件
├── ntusetup.tex                    // 模板設定
├── ntuthesis.cls                   // 模板文件
└── ...
```

## License

Licensed under the MIT License, Copyright © 2017-present Hsins. Modified by withworkSC. 
