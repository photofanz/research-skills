學員專屬的 research skills（含公開的 skills），供學習 & 參考使用。

請自行確認執行結果。

## 安裝方式

- 將壓縮檔解壓縮到某個目錄內。例如： research_skills_vip_folder
- 切換你的工作目錄（也就是要安裝 agent skill 的 專案目錄）
- 在工作目錄下執行下方指令：
	- npx skills add {research_skills_vip_folder 的完整路徑}

## skills 說明

### 免費公開

- general-reader-simulator： 一般讀者模擬
	- 用途：
		- 模擬無特殊知識背景的讀者來閱讀指定的文章，並且可進一步要求產生【作者意圖-讀者理解對齊報告】
	- skill 設計背景：
	  [研究者的知識詛咒：Agent 能不能幫我們看見自己看不見的論文問題？ | Ted 的 AI 學術顧問所](https://www.research-ai.cc/blog/curse-of-knowledge-research-agent)
	- 用法範例：
		- 方法一：
			- prompt1：
				- /general-reader-simulator 幫我分析我這篇文章： {文章檔名}
			- prompt2：
				- 讀者與我的意圖對齊狀況如何？
		- 方法二：
			- prompt1：/general-reader-simulator 幫我分析我這篇文章： {文章檔名}。我文章撰寫的目標為：{文章意圖說明文件檔名}
	- 備註
		- 文章意圖說明文件，可參考 skill 內： author-intent-card.md

### 學員專屬

- causal-chain-assumption-audit： 因果鏈與假設清單分析
	- 用途：
		- 此 agent skill 會掃描指定的檔案 or 網頁部落格內容內，關鍵的 段落主張 & 核心主張的骨幹後，協助分析選定主張的 因果鏈結構 以及進行否定測試後的假設支撐度清單。
	- skill 設計背景：
		- 待補
	- 用法範例：
		- 會有兩個階段，第一階段先掃描 & 確認核心主張 & 骨幹，啟動提示詞範例：
			-   /causal-chain-assumption-audit {檔案路徑&名稱}
			- 後續按照提示回覆