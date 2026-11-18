# MZ-2000 / MZ-2200 DVI-D Video Card (WeAct RP2350B)

[日本語](#日本語) | [English](#english)

---

<a id="日本語"></a>
## 🇯🇵 日本語

**WeAct RP2350B core board** を使用した、SHARP MZ-2000 / MZ-2200 用の DVI-D 出力ビデオカードプロジェクトです。

### 📌 現在の公開状況（Status）
*   ✅ **3Dモデル（コネクタ筐体）**：先行公開中（`3d-models/WAGRAM0123VN.stl`）
*   🚧 **回路図・基板データ（PCB）**：準備中
*   🚧 **ファームウェア**：準備中

### 🔌 互換コネクタの3Dデータと組み立て（3D Models & Assembly）
廃盤となった拡張コネクタ **HIROSE `PCN5-53ST-1.27W`** と物理的な互換性を持つオリジナル設計のコネクタ筐体（`3d-models/WAGRAM0123VN.stl`）です。

#### 🖨️ 推奨3Dプリント設定 (Bambu Lab A1 mini)
*   **ノズル径**：**0.2mm**（微細ピッチのため必須）
*   **配置・サポート**：基板側が下、サポートは「通常（Normal）」

#### 🛠️ 使用部品・組み立て方法
秋月電子のパーツを加工して計44本のコンタクトピンを組み上げます。

*   **使用部品（秋月電子通商）**：
    1. **[丸ピンIC用ソケット (シングル40P) 1×40](https://akizukidenshi.com)**（型番：`6604S-40` / 通販コード：`101591`）× 2本
    2. **[分割ロングピンソケット 1×42 (42P)](https://akizukidenshi.com)**（型番：`FHU-1x42SG` / 通販コード：`105779`）× 2本
*   **組み立て手順**（[参考ポスト](https://x.com/gaiyaseki/status/2123045014657982490)）：コンタクトの抜き取り・曲げ加工を行い、丸ピンソケットと組み合わせて3Dプリント筐体に44本を植え込みます。

### ⚠️ 免責事項・ライセンス
*   **非公式設計・自己責任**：ヒロセ電機株式会社およびシャープ株式会社とは無関係であり、利用による損害の責任は負いません。
*   **ライセンス**：[MIT License](LICENSE)

---

<a id="english"></a>
## 🇺🇸 English

A DVI-D video output card project for the **SHARP MZ-2000 / MZ-2200**, powered by the **WeAct RP2350B core board**.

### 📌 Project Status
*   ✅ **3D Models (Custom Connector Housing)**: Available now (`3d-models/WAGRAM0123VN.stl`)
*   🚧 **Schematics & PCB Design**: Work in progress
*   🚧 **Firmware**: Work in progress

### 🔌 About the Compatible Connector 3D Data & Assembly
A 3D-printable custom housing (`3d-models/WAGRAM0123VN.stl`) physically compatible with the discontinued **HIROSE `PCN5-53ST-1.27W`** slot connector.

#### 🖨️ Recommended 3D Print Settings (Bambu Lab A1 mini)
*   **Nozzle Size**: **0.2mm** (Required for fine pitch)
*   **Orientation & Support**: PCB side facing down, Normal support

#### 🛠️ Parts & Assembly Notes
Assembled by modifying 44 pins using parts from Akizuki Denshi:

*   **Required Parts**:
    1. **[Round Pin IC Socket (Single 40P) 1×40](https://akizukidenshi.com)** (Part No: `6604S-40` / Order Code: `101591`) × 2
    2. **[Breakaway Long Pin Socket 1×42 (42P)](https://akizukidenshi.com)** (Part No: `FHU-1x42SG` / Order Code: `105779`) × 2
*   **Assembly Overview** ([Reference Post](https://x.com/gaiyaseki/status/2123045014657982490)): Extract contacts, bend tabs, combine with round-pin sockets, and insert 44 contacts into the housing.

### ⚠️ Disclaimer & License
*   **Unofficial / Use at Your Own Risk**: Not affiliated with Hirose Electric or Sharp. The author assumes no liability for damage.
*   **License**: Released under the [MIT License](LICENSE).
