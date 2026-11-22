# WA-GRAM0123 — MZ-2000 / MZ-2200 DVI-D Video Card (WeAct RP2350B)

[日本語](#日本語) | [English](#english)

---

<a id="日本語"></a>
## 🇯🇵 日本語

**WeAct RP2350B core board** を使用した、SHARP MZ-2000 / MZ-2200 用の DVI-D 出力ビデオカードプロジェクトです。

### 📌 公開状況
| 内容 | 状況 |
|---|---|
| 互換コネクタ：3Dプリント用筐体（STL） | ✅ 公開中 |
| 互換コネクタ：KiCad シンボル・フットプリント | ✅ 公開中 |
| 回路図・基板データ（PCB） | 🚧 準備中 |
| ファームウェア | 🚧 準備中 |

### 📁 ファイル構成
```
3dmodels/
  WAGRAM0123CN.FCStd        互換コネクタの筐体（FreeCAD）
  WAGRAM0123CN.stl          互換コネクタの筐体（3Dプリント用）
  kicad/
    WAGRAM0123CN.kicad_sym  シンボルライブラリ
    WAGRAM0123CN.pretty/    フットプリントライブラリ
    WAGRAM0123CN.step       互換コネクタの筐体（KiCad 3Dビューワー等用）
LICENSE                     CERN-OHL-P-2.0
README.md
```

### 🔌 互換コネクタについて
廃番となった拡張コネクタ **HIROSE `PCN5-53ST-1.27W`** の代わりに使える、オリジナル設計のコネクタです。
FreeCADやKiCadを使用しはじめたばかりの頃に制作したものなので、雑な部分がかなりあります。
特にFreeCADのデータはひどいです。ご了承の上ご使用ください。

- **外形**：高さを除いて `PCN5-53ST-1.27W` とほぼ同一です。高さは異なるため、ケースや隣のスロットと干渉しないか確認してください。
- **コンタクト**：市販のピンソケットを加工したものを使います。基板側53本、コネクタ接続側44本。本機で使用していない信号は接続していません。
- **設計**：内部構造、シンボル、フットプリントは作者のオリジナル設計です。

### 🧩 KiCad ライブラリ
- **対応バージョン**：KiCad 10 で作成しています。それより古い KiCad では開けません。
- **使い方**：`3dmodels/kicad/WAGRAM0123CN.kicad_sym` をシンボルライブラリとして、`3dmodels/kicad/WAGRAM0123CN.pretty` をフットプリントライブラリとして登録してください。プロジェクト固有のライブラリとして登録すると、プロジェクトと一緒に持ち運べます。
- **注意**：基板を発注する前に、フットプリントの寸法とピン配置をご自身の設計と照合してください。

### 🖨️ 推奨3Dプリント設定（Bambu Lab A1 mini）
- **ノズル径**：**0.2mm**（ピッチが細かいため必須）
- **配置・サポート**：プリントは基板側を上、コネクタ接続側を下にし、サポートは「通常（Normal）」

### 🛠️ 使用部品・組み立て
市販のパーツを加工しコンタクトを組み上げます。作者が使用したのは秋月電子通商で販売されているものです。

| 部品 | メーカー型番 | 通販コード | 数量 |
|---|---|---|---|
| [丸ピンIC用ソケット (シングル40P) 1×40](https://akizukidenshi.com/catalog/g/g101591/) | `6604S-40` | 101591 | 2個 |
| [分割ロングピンソケット 1×42 (42P)](https://akizukidenshi.com/catalog/g/g105779/) | `FHU-1x42SG` | 105779 | 2個 |

**組み立て手順**（[参考ポスト](https://x.com/gaiyaseki/status/2123045014657982490)）：コンタクトの抜き取り・曲げ加工を行い、丸ピンソケットと組み合わせて、3Dプリントした筐体に埋め込みます。

### ⚠️ 免責事項
- 本プロジェクトは個人による非公式の設計です。ヒロセ電機株式会社およびシャープ株式会社とは関係ありません。
- 利用は自己責任でお願いします。本機器・データの使用によって生じた損害について、作者は責任を負いません。
- 記載している会社名・製品名は、各社の商標または登録商標です。

### 📜 ライセンス
このリポジトリで公開しているデータ（3Dモデル・シンボル・フットプリント）は、**[CERN Open Hardware Licence Version 2 - Permissive（CERN-OHL-P-2.0）](LICENSE)** で公開しています。商用を含め、自由に利用・改変・再配布・製品化できます。

- **改変して再配布するとき**：著作権表示とライセンス表示を残し、改変した旨・日付・改変内容の概要を書き添えてください。
- **製品として配布するとき**：受け取った人がこれらの表示を確認できるようにしてください（例：このリポジトリのURLを添える）。

回路図・基板データ・ファームウェアのライセンスは、公開時に明記します。

Copyright © 2026 Gaiyaseki — <https://github.com/Gaiyaseki/WA-GRAM0123>
`SPDX-License-Identifier: CERN-OHL-P-2.0`

---

<a id="english"></a>
## 🇺🇸 English

A DVI-D video output card project for the **SHARP MZ-2000 / MZ-2200**, powered by the **WeAct RP2350B core board**.

### 📌 Project Status
| Item | Status |
|---|---|
| Compatible connector: 3D-printable housing (STL) | ✅ Available |
| Compatible connector: KiCad symbol & footprint | ✅ Available |
| Schematics & PCB design | 🚧 Work in progress |
| Firmware | 🚧 Work in progress |

### 📁 Repository Layout
```
3dmodels/
  WAGRAM0123CN.FCStd        Connector housing (FreeCAD)
  WAGRAM0123CN.stl          Connector housing (for 3D printing)
  kicad/
    WAGRAM0123CN.kicad_sym  Symbol library
    WAGRAM0123CN.pretty/    Footprint library
    WAGRAM0123CN.step       Connector housing (for the KiCad 3D viewer, etc.)
LICENSE                     CERN-OHL-P-2.0
README.md
```

### 🔌 About the Compatible Connector
An original connector design that can replace the discontinued **HIROSE `PCN5-53ST-1.27W`** expansion connector.
These files were made when I had just started using FreeCAD and KiCad, so quite a few parts of them are rough.
The FreeCAD data in particular is very messy. Please keep this in mind when using them.

- **Outline**: Nearly identical to the `PCN5-53ST-1.27W` except for its height. Because the height differs, check clearance against the case and adjacent slots.
- **Contacts**: Made by modifying off-the-shelf pin sockets: 53 pins on the PCB side and 44 contacts on the mating side. Signals not used by this card are not connected.
- **Design**: The internal structure, symbol and footprint are the author's original designs.

### 🧩 KiCad Libraries
- **Version**: Created with KiCad 10. Older versions of KiCad cannot open these files.
- **Usage**: Add `3dmodels/kicad/WAGRAM0123CN.kicad_sym` as a symbol library and `3dmodels/kicad/WAGRAM0123CN.pretty` as a footprint library. Adding them as project-specific libraries keeps them with your project.
- **Note**: Verify the footprint dimensions and pin assignment against your own design before ordering boards.

### 🖨️ Recommended 3D Print Settings (Bambu Lab A1 mini)
- **Nozzle size**: **0.2 mm** (required for the fine pitch)
- **Orientation & support**: Print with the PCB side up and the mating side down, Normal support

### 🛠️ Parts & Assembly
The contacts are made by modifying off-the-shelf parts. The author used parts sold by Akizuki Denshi.

| Part | Manufacturer P/N | Akizuki code | Qty |
|---|---|---|---|
| [Round-pin IC socket, single row 1×40](https://akizukidenshi.com/catalog/g/g101591/) | `6604S-40` | 101591 | 2 |
| [Breakaway long-pin socket 1×42](https://akizukidenshi.com/catalog/g/g105779/) | `FHU-1x42SG` | 105779 | 2 |

**Assembly overview** ([reference post](https://x.com/gaiyaseki/status/2123045014657982490)): Extract and bend the contacts, combine them with the round-pin sockets, and embed them in the printed housing.

### ⚠️ Disclaimer
- This is an unofficial personal design, not affiliated with Hirose Electric Co., Ltd. or Sharp Corporation.
- Use at your own risk. The author accepts no liability for any damage arising from the use of this hardware or data.
- Company and product names mentioned here are trademarks or registered trademarks of their respective owners.

### 📜 License
The data published in this repository (3D model, symbol and footprint) is released under the **[CERN Open Hardware Licence Version 2 - Permissive (CERN-OHL-P-2.0)](LICENSE)**. You may use, modify, redistribute and manufacture it freely, including for commercial purposes.

- **If you redistribute a modified version**: keep the copyright and licence notices, and add a note stating that you modified it, with the date and a brief description of the changes.
- **If you distribute products**: make sure recipients can access these notices (e.g. by providing the URL of this repository).

The licences for the schematics, PCB data and firmware will be stated when they are released.

Copyright © 2026 Gaiyaseki — <https://github.com/Gaiyaseki/WA-GRAM0123>
`SPDX-License-Identifier: CERN-OHL-P-2.0`
