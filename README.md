# Decoding Social Sentiment in DAO: A Comparative Analysis of Blockchain Governance Communities

## *Supplementary resources, data, and code*
by **Yutong Quan**, **Xintong Wu**, **Wanlin Deng** and **Luyao Zhang***

(* *corresponding authors*)

## Table of Contents
- [Data](https://github.com/SciEcon/BlockchainSentiment2023/tree/main#data)
- [Code](https://github.com/SciEcon/BlockchainSentiment2023/tree/main#code)
- [Reference](https://github.com/SciEcon/BlockchainSentiment2023/tree/main#references)
## Data
### Collected Data
- **Data File Information**

| **DeFi Protocols** | **Data File** | **Channel** | **Start Date** | **End Date** | **Message Count** |
| -------------------| ------- | ------- | ------- | ------- | ------- |
| Aave               | Aave Community - ┌────AAVE Token────┐ - 📜governance [605528212239286312].csv | governance | 8/2/2019 | 7/27/2023 | 3,844 |
| Uniswap            | Uniswap - Governance - 🏛│governance [755969053280960533].csv | governance | 9/17/2020 | 8 13/2023 | 11,583 |
| Curve DAO          | Curve Finance - General - curve-governance [745257323487953036].csv | curve-governance | 8/18/2020 | 8/15/2023 | 8,774 |
| Aragon             | Aragon 🦅 - DAO Builders - dao-builders-chat [1036975360551702568].csv | dao-builders-chat | 11/20/2022 | 8/15/2023 | 702 |
| yearn.finance      | Yearn Talk - general - 🗳governance [734805853768777738].csv | governance | 7/20/2020 | 8/2/2023 | 7,214 |
| Merit Circle       | Merit Circle - 💬 Chats & Voice──────────── - ╭💬・general-chat [942785405617582110].csv | general-chat | 2/14/2022 | 8/15/2023 | 34,786 |
| Balancer           | Balancer - 🏡 _ Discussions - 💬︲general-chat [638460494168064025].csv | general-chat | 11/29/2019 | 8/15/2023 | 51,707 |

- **Data Dictionary**

| **Variable Name**	| **Unit**	| **Data Type**	| **Description** |
| ------- | ------- | ------- | ------- |
| AuthorID	| Count | int64 | This identifier uniquely distinguishes the authors of the discussions, allowing for tracking and attribution. |
| Author | Name |int64 | The name or username of the discussion participants. |
| Date_original | Minutes | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in minutes). |
| Date | Days | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in days). |
| Content | Text | int64 | The textual content of the discussions, including messages, comments, and replies. |
| Attachments | File/Link/Image | int64 | Information regarding any attached files, images, or media shared within the discussions. |
| Reactions | Emoji | int64 | A record of reactions, such as emojis, associated with each discussion, offering insights into community engagement and sentiment. |

### Analyzed Data
- **Data File Information**

| **DeFi Protocols** | **Data File** | **Description** |
| ------- | ------- | ------- |
| **Aave** | aave_cleaned_discord | This file provided the preprocessed content from the collected dataset of Aave. | 
| | aave_daily_sentiment | This file contains the daily sentiment score of discussion in the Aave community on Discord. | 
| | aave_user_sentiment | This file includes the user-based sentiment score of discussion in the Aave community on Discord. | 
| | aave_volume_discord | This file presents the daily discussion volume for the Aave community on Discord. | 
| **Uniswap** | uniswap_cleaned_discord | This file provided the preprocessed content from the collected dataset of Uniswap. | 
| | uniswap_daily_sentiment | This file includes the user-based sentiment score of discussion in the Uniswap community on Discord. | 
| | uniswap_user_sentiment | This file presents the daily discussion volume for the Uniswap community on Discord. | 
| | uniswap_volume_discord | This file presents the daily discussion volume for the Uniswap community on Discord. | 
| **Curve Dao** | curve_cleaned_discord | This file provided the preprocessed content from the collected dataset of Curve Dao. | 
| | curve_daily_sentiment | This file includes the user-based sentiment score of discussion in the Curve Dao community on Discord. | 
| | curve_user_sentiment | This file presents the daily discussion volume for the Curve Dao community on Discord. | 
| | curve_volume_discord | This file presents the daily discussion volume for the Curve Dao community on Discord. | 
| **Aragon** | aragon_cleaned_discord | This file provided the preprocessed content from the collected dataset of Aragon. | 
| | aragon_daily_sentiment | This file includes the user-based sentiment score of discussion in the Aragon community on Discord. | 
| | aragon_user_sentiment | This file presents the daily discussion volume for the Aragon community on Discord. | 
| | aragon_volume_discord | This file presents the daily discussion volume for the Aragon community on Discord. | 
| **Yearn Finance** | yearnfinance_cleaned_discord | This file provided the preprocessed content from the collected dataset of Yearn Finance. | 
| | yearnfinance_daily_sentiment | This file includes the user-based sentiment score of discussion in the Yearn Finance community on Discord. | 
| | yearnfinance_user_sentiment | This file presents the daily discussion volume for the Yearn Finance community on Discord. | 
| | yearnfinance_volume_discord | This file presents the daily discussion volume for the Yearn Finance community on Discord. | 
| **Merit Circle** | meritcircle_cleaned_discord | This file provided the preprocessed content from the collected dataset of Merit Circle. | 
| | meritcircle_daily_sentiment | This file includes the user-based sentiment score of discussion in the Merit Circle community on Discord. | 
| | meritcircle_user_sentiment | This file presents the daily discussion volume for the Merit Circle community on Discord. | 
| | meritcircle_volume_discord | This file presents the daily discussion volume for the Merit Circle community on Discord. | 
| **Balancer** | balancer_cleaned_discord | This file provided the preprocessed content from the collected dataset of Balancer. | 
| | balancer_daily_sentiment | This file includes the user-based sentiment score of discussion in the Balancer community on Discord. | 
| | balancer_user_sentiment | This file presents the daily discussion volume for the Balancer community on Discord. | 
| | balancer_volume_discord | This file presents the daily discussion volume for the Balancer community on Discord. | 

- **Data Dictionary**

| **File Classification** | **Variable Name**	| **Unit**	| **Data Type**	| **Description** |
| ------- | ------- | ------- | ------- | ------- |
| *DeFi*_cleaned_discord | AuthorID	| Count | int64 | This identifier uniquely distinguishes the authors of the discussions, allowing for tracking and attribution. |
| | Author | Name |int64 | The name or username of the discussion participants. |
| | Date_original | Minutes | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in minutes). |
| | Date | Days | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in days). |
| | Content | Text | int64 | The textual content of the discussions, including messages, comments, and replies. |
| | Attachments | File/Link/Image | int64 | Information regarding any attached files, images, or media shared within the discussions. |
| | Reactions | Emoji | int64 | A record of reactions, such as emojis, associated with each discussion, offering insights into community engagement and sentiment. |
| | Preprocessed | Text | int64 | The preprocessed textual content of the discussions with lowercasing, URL removal, special character removal, tokenization, stopword removal, and punctuation removal. |
| *DeFi*_daily_sentiment | Date | Days | datetime64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in days). |
| | Sentiment Score | Range=[-1,1] | int64 | The calculated average sentiment score for each day with discussion occurred. |
| *DeFi*_user_sentiment | AuthorID | Count | int64 | This identifier uniquely distinguishes the authors of the discussions, allowing for tracking and attribution. |
| | Average_Sentiment_Score | Range=[-1,1] | int64 | The calculated average sentiment score for each author who participated in the discussion. |
| *DeFi*_volume_discord | Date | Days | datetime64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in days). |
| | Discord Volume | Count | int64 | The daily discussion volume on DeFi protocols' Discord channel.|

## Code
| **DeFi Protocols** | **Google Colab File Name**|
| ------- | ------- |
| Aave | Aave.ipynb |
| Uniswap | Uniswap.ipynb |
| Curve Dao | Curve_Dao.ipynb |
| Aragon | Aragon.ipynb |
| yearn.finance | yearn_finance.ipynb |
| Merit Circle | Merit_Circle.ipynb |
| Balancer | Balancer |

## References
**Data Reference:** Discord (https://discord.com/)

**Code Reference:** Tyrrrz/DiscordChatExporter (https://github.com/Tyrrrz/DiscordChatExporter)



