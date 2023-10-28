# Decoding Social Sentiment: A Comprehensive Analysis of Blockchain Governance Communities

## *Supplementary resources, data, and code*
by **Yutong Quan**, **Xintong Wu**, **Wanlin Deng** and **Luyao Zhang***

(* *corresponding authors*)

## Data
### Collected Data
- **Data File Information**

| **DeFi Protocols** | **Data File** | **Channel** | Start Date | End Date | Message Count|
| -------------------| ------- | ------- | ------- | ------- | ------- |
| Aave               | Aave Community - ┌────AAVE Token────┐ - 📜governance [605528212239286312].csv | governance | 8/2/2019 | 7/27/2023 | 3,844 |
| Uniswap            | Uniswap - Governance - 🏛│governance [755969053280960533].csv | governance | 9/17/2020 | 8 13/2023 | 11,583 |
| Curve DAO          | Curve Finance - General - curve-governance [745257323487953036].csv | curve-governance | 8/18/2020 | 8/15/2023 | 8,774 |
| Aragon             | Aragon 🦅 - DAO Builders - dao-builders-chat [1036975360551702568].csv | dao-builders-chat | 11/20/2022 | 8/15/2023 | 702 |
| yearn.finance      | Yearn Talk - general - 🗳governance [734805853768777738].csv | governance | 7/20/2020 | 8/2/2023 | 7,214 |
| ------- | ------- | ------- | ------- | ------- |
| Merit Circle       | Merit Circle - 💬 Chats & Voice──────────── - ╭💬・general-chat [942785405617582110].csv | general-chat | 2/14/2022 | 8/15/2023 | 34,786 |
| Balancer           | Balancer - 🏡 _ Discussions - 💬︲general-chat [638460494168064025].csv | general-chat | 11/29/2019 | 8/15/2023 | 51,707 |

- **Data Dictionary**

| Variable Name	| Unit	| Data Type	| Description |
| ------- | ------- | ------- | ------- |
| AuthorID	| Count | int64 | This identifier uniquely distinguishes the authors of the discussions, allowing for tracking and attribution. |
| Author | Name |int64 | The name or username of the discussion participants. |
| Date_original | Minutes | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in minutes). |
| Date | Days | int64 | The timestamp indicates when each discussion occurred, providing a temporal dimension to the dataset (shown in days). |
| Content | Text | int64 | The textual content of the discussions, including messages, comments, and replies. |
| Attachments | File/Link/Image | int64 | Information regarding any attached files, images, or media shared within the discussions. |
| Reactions | Emoji | int64 | A record of reactions, such as emojis, associated with each discussion, offering insights into community engagement and sentiment. |

### Analyzed Data

