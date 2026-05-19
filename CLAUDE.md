# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 常用命令

- **构建**: `npm run build` （如果使用 npm）或 `make`（如果存在 Makefile）
- **代码检查 / Lint**: `npm run lint` 或 `make lint`
- **运行全部测试**: `npm test` 或 `make test`
- **运行单个测试**: `npm test -- <test‑file>` 或 `make test TEST=<test‑file>`
- **启动开发服务器**: `npm start` 或 `make dev`

> 根据实际项目所使用的构建工具、包管理器或测试框架，替换上述占位命令。

## 项目概览与架构

> 项目为空，占位结构如下，随后请根据实际代码补充。

- `src/` – 业务代码根目录，建议使用 TypeScript/JavaScript（或其他语言）组织模块。
- `tests/` – 单元测试和集成测试所在目录。
- `scripts/` – 项目维护脚本，例如构建、部署、代码生成等。
- `README.md` – 项目概述、快速开始、依赖说明等文档入口。
- `package.json` / `requirements.txt` / `pyproject.toml` – 项目依赖与脚本声明。

如果项目使用 **Cursor** 或 **Copilot**，请在根目录下放置相应规则文件：
- `.cursor/rules/` – Cursor 规则目录。
- `.github/copilot-instructions.md` – Copilot 指令文档。

## 开发建议

- 在提交前运行 **lint** 与 **测试**，保持代码风格一致并防止回归。
- 使用 **Git 分支** 开发新功能或 bug‑fix，完成后提交 PR 并通过 CI 检查。
- 如需调试单元测试，可使用 IDE 的调试功能或在命令行加上 `--watch`、`--debug` 参数（视测试框架而定）。

## 记录与更新

- 当项目结构、依赖或常用命令发生变化时，请及时更新本文件。
- 若项目添加了特定的 **Cursor** / **Copilot** 规则，请在本节列出关键规则或引用对应文件。

---

*该文件为占位模板，后续请根据实际项目内容补充完善。*