# 🐼 Panda BT 2.0 Helper

![GitHub package.json version](https://img.shields.io/github/package-json/v/ryulurala/vscode-pandabt2-helper?style=for-the-badge)
![GitHub License](https://img.shields.io/github/license/ryulurala/vscode-pandabt2-helper?style=for-the-badge)

[![Visual Studio Marketplace Link](https://img.shields.io/badge/Visual%20Studio%20Marketplace-black?style=for-the-badge&logo=visualstudiocode)](https://marketplace.visualstudio.com/items?itemName=ryulurala.pandabt-helper)
![Visual Studio Marketplace Downloads](https://img.shields.io/visual-studio-marketplace/d/ryulurala.pandabt-helper?style=for-the-badge)
![Visual Studio Marketplace Installs](https://img.shields.io/visual-studio-marketplace/i/ryulurala.pandabt-helper?style=for-the-badge)

## Overview

**Panda BT 2.0 Helper**는 [Panda BT 2 (Unity Asset)](https://assetstore.unity.com/packages/tools/behavior-ai/panda-bt-2-274073)를 사용하는 개발자가 Visual Studio Code에서 `.pbt` 파일을 더 편리하게 편집할 수 있도록 만든 확장입니다.

이 확장은 Panda BT 2.0 사용자 경험을 개선하기 위해 직접 개발되었으며, **텍스트 하이라이팅**과 **자동 포맷팅**을 통해 보다 빠르고 일관된 BT 스크립팅 작업을 지원합니다.

## ✨ Features

### ✅ 텍스트 하이라이팅

- `.pbt` 확장자를 위한 Panda BT 2 전용 하이라이팅 규칙을 제공합니다.
- 커맨드, 태스크, 주석 등의 가독성을 향상시킵니다.

### ✅ 포맷팅 (Format on Save)

- VS Code에서 저장 시 자동으로 문서를 포맷합니다.
- 코드 스타일을 일관되게 유지할 수 있습니다.

## 🖥 Requirements

- Visual Studio Code **v1.99.0 이상**
- Node.js **v22.14.0** (Extension 빌드 기준)

## ⚙ Commands

| Command Name                    | Description                                                                                                                                        |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Panda BT: Apply Default Color` | 개발자가 지정한 기본 색상 설정으로 되돌립니다. VS Code의 설정(`settings.json`)에서 텍스트 컬러를 초기화할 수 있습니다. 단축키는 제공되지 않습니다. |

## 🔧 Configuration

설치하면 `settings.json`에 자동으로 아래 설정이 반영됩니다:

```json
"editor.tokenColorCustomizations": {
  "textMateRules": [
    {
      "scope": "pandabt.tree",
      "settings": {
        "foreground": "#E06C75",
        "fontStyle": "bold"
      }
    },
    ...
  ]
}
```
