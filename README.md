# javascript-calculator-precourse

## 📜구현 기능 목록

### 1. 입력 유효성 검사 🆗

**파일명**: `is_valid.js`

**함수 및 기능**

- **`validateInput(INPUT)`** - 사용자의 입력이 **비어있을 경우** `[ERROR] 입력값이 없습니다.` 에러를 발생시킵니다.
- **`validateNumber(VALUE)`** - 전달받은 값이 **숫자가 아니거나 음수가 포함된 경우** `[ERROR] 입력이 올바르지 않습니다.` 에러를 발생시킵니다.

---

### 2. 구분자 파싱 ✅

**파일명**: `delimiter_parser.js`

**함수 및 기능**

- **`parseInputWithDelimiter(INPUT)`** - **커스텀 구분자**(`//구분자\n`)가 포함된 입력인지 확인하고, 이에 따라 문자열을 **분리**합니다.

  - 기본 구분자: 쉼표(,), 콜론(:)
  - 커스텀 구분자 예시: `//;\n1;2;3` → `[1, 2, 3]`

---

### 3. 덧셈 수행 ➕

**파일명**: `calculator.js`

**함수 및 기능**

- **`sum(NUMBERS)`** - 문자열로부터 분리된 숫자 배열을 **`int`형으로 변환**하고, 유효성 검사 후 합산합니다.

  - 예시: `[1, 2, 3]` → `6`
  - 유효하지 않은 값이 포함된 경우 에러를 발생시킵니다.
