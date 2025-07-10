# 📦 Version Releases

This project follows **Semantic Versioning (SemVer)** for release naming.

---

## 🧱 Basic Format: `vMAJOR.MINOR.PATCH`

**Examples:**

- `v1.0.0`
- `v1.0.1`
- `v1.1.1`

---

## 🚧 Pre-release: `vMAJOR.MINOR.PATCH-<BETA|RC|SNAPSHOT>.<number>`

**Examples:**

- `v1.0.0-beta.1`
- `v1.0.0-beta.2`
- `v1.2.3-rc1`
- `v1.2.3-SNAPSHOT`

> 🔹 `SNAPSHOT` versions indicate unstable or in-progress builds.

---

## 📮 Post-release: `vMAJOR.MINOR.PATCH-post.<number>`

**Examples:**

- `v1.2.3-post.1`
- `v1.2.3-post.2`

---

## 💻 Local Dev: `vMAJOR.MINOR.PATCH+LOCAL`

**Examples:**

- `v1.0.0+local`
- `v1.1.0+local`

---

## 📐 Range Versions

### Caret (`^`):

Represents compatible versions within the same major version.

- `^1.2.3` → `>=1.2.3 <2.0.0`

### Tilde (`~`):

Represents patch-level compatibility within the same minor version.

- `~1.2.3` → `>=1.2.3 <1.3.0`

---

## 🧠 Terminology

| Term     | Description                      |
| -------- | -------------------------------- |
| MAJOR    | Breaking changes                 |
| MINOR    | Backward-compatible features     |
| PATCH    | Bug fixes and small enhancements |
| SNAPSHOT | In-progress development builds   |

---
