# Zhuang-CN-S2TT-Dataset
Zhuang-CN S2TT is a Zhuang–Chinese speech-to-text parallel dataset, which constructed through a recording and processing  pipeline that includes manual recording, automatic audio segmentation, text annotation, and alignment verification. 

# 1.壮语语音数据集示例 / Zhuang-CN-S2TT Dataset Example
本仓库提供一个壮语语音数据集的示例，包含语音录音及其对应的转录与元数据。  
该数据旨在支持壮语语音到中文文本翻译、方言学研究以及少数民族语言资源建设。

This repository provides a sample of a Zhuang (壮语) speech dataset, including audio recordings and corresponding transcriptions in TSV format.  
It is intended for research in Zhuang-to-Chinese speech-to-text translation (S2TT), dialectology research, and the development of language resources for minority languages.

---

## 2.语言信息 / Language Information
- **语言名称 (Language Name)：** 壮语（Zhuang）  
- **语系 (Language Family)：** 壮侗语系-侗台语族-壮傣语支（Kra–Dai language family - Tai–Kadai branch - Zhuang–Tai subgroup）  
- **方言类型 (Dialect)：** 壮语南部方言中的德靖土语，以广西靖西、德保、那坡话为主。
The recordings in this dataset represent Dejing local variety of the Southern Zhuang dialect, mainly based on the Jingxi, Debao, and Napo varieties in Guangxi, China.

---

## 3.数据集内容 / Dataset Description
该示例数据集包含以下内容：
- **音频文件（`audio/*.wav`）**：录制的壮语语音样本  
- **转录文件（`zhuang_demo.tsv`）**：包含音频文件路径及相关元数据的 TSV 文件  

The sample dataset includes:
- **Audio files** (`audio/*.wav`): Speech recordings of Zhuang language.
- **Transcriptions** (`zhuang_demo.tsv`): Tab-separated files containing metadata and text transcriptions.

**字段说明 / TSV Columns:**
| 字段名 (Field) | 含义 (Description) |
|----------------|--------------------|
| `speaker_id` | 说话人编号 (Speaker ID) |
| `audio path` | 音频文件路径 (Audio file path) |
| `sentence` | 壮语句子转录 (Transcribed sentence) |
| `up_votes` | 有效标注投票数 (Quality upvotes) |
| `down_votes` | 无效标注投票数 (Quality downvotes) |
| `age` | 说话人年龄 (Age of the speaker) |
| `gender` | 说话人性别 (Gender) |
| `accent` | 方言/口音信息 (Accent information) |

**示例 (Example):**
| speaker_id | audio path | sentence | up_votes | down_votes | age | gender | accent |
|-------------|-------------|-----------|-----------|-------------|------|--------|--------|
| speaker01 | speaker01-c21-001.wav | 明天我去北京旅游，这次在北京一共待七天。 | 1.0 | 0.0 | 24.0 | female | — |

---

## 4.文件结构 / Directory Structure
zhuang-speech-sample/
├── audio/
│ ├── speaker01-c21-001.wav
├── zhuang_demo.tsv
└── README.md

---

## 5.使用说明 / Usage
数据集格式与 [fairseq](https://github.com/facebookresearch/fairseq) 的语音到文本翻译的数据加载方式兼容。可参考 fairseq 官方文档或示例进行预处理与模型训练。

The dataset format is compatible with [fairseq](https://github.com/facebookresearch/fairseq) for speech recognition.  
Please refer to the fairseq documentation for preprocessing and training examples.

---

## 6.未来计划 / Future Work
我们计划在未来版本中：
（1）增加更多说话人样本（不同年龄与性别）；
（2）扩充句子数量，覆盖更多日常语域与语音现象；
（3）添加汉语和英文翻译字段；
（4）发布完整的壮语语音数据集，并提供标准的数据集划分。

Future updates will include:
(1) More speakers across different demographics;
(2) Expanded sentence coverage and linguistic diversity;
(3) Additional translation and phonetic annotation fields;
(4) Full-scale Zhuang speech corpus with S2TT-ready splits.

---

## 7.许可与授权 / License and Citation
## License
本数据集采用 CC BY 4.0 许可协议（https://creativecommons.org/licenses/by/4.0/），使用者可自由分享与修改，但需注明来源。

This dataset is released under the [CC BY 4.0 License] https://creativecommons.org/licenses/by/4.0/).  
You are free to share and adapt the material, provided appropriate credit is given.

## Citation
如果您使用了本数据集，请引用如下：
Haina Nong．(2025)．Zhuang-CN S2TT Dataset Example．GitHub．https://github.com/nonghaihai/Zhuang-CN-S2TT-Dataset

If you use this dataset, please cite as:
> Haina Nong, (2025). *Zhuang-CN S2TT Dataset Example*. GitHub Repository: https://github.com/nonghaihai/Zhuang-CN-S2TT-Dataset

---

## 8.致谢 / Acknowledgments
感谢所有参与录音与标注的壮语母语者。
本项目旨在促进少数民族语言的数字化与科技应用研究。

Special thanks to the native Zhuang speakers who contributed their voices and time.
This project supports language preservation and open research in under-resourced languages.

---

## 9.联系方式 / Contact
如有问题或合作意向，请联系：2313391016@st.gxu.edu.cn

For questions or collaborations, please contact: 2313391016@st.gxu.edu.cn
