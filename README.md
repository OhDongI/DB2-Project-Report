# 요양원 관리 시스템 - DB 프로젝트

## 📌 프로젝트 개요

이 프로젝트는 **"DB 설계 및 구현 2"** 과목의 최종 데이터베이스 설계 팀프로젝트로, 요양원의 다양한 운영 관리를 효율적으로 지원하기 위한 데이터베이스 시스템을 개발하는 데 목적이 있습니다. 기존의 수기 기록 방식에서 데이터베이스 중심으로 전환하여 정보 접근성과 신뢰성을 향상시키고 운영 효율성을 극대화합니다.

---

## 📋 목차
1. [프로젝트 목적](#-프로젝트-목적)
2. [시스템 주요 기능](#-시스템-주요-기능)
3. [데이터베이스 설계](#-데이터베이스-설계)
4. [SQL 쿼리](#-sql-쿼리)
5. [사용 방법](#-사용-방법)
6. [라이선스](#-라이선스)

---

## 🎯 프로젝트 목적

이 프로젝트는 요양원의 관리 시스템을 개선하여 다음과 같은 주요 목표를 달성합니다:
- **건강 기록 관리**: 입소자의 건강 데이터(혈압, 체온, 약물 기록 등)를 효율적으로 저장 및 관리
- **직원 관리**: 직원의 일정, 업무 배정 및 역할을 체계적으로 관리
- **생활 지원 서비스 기록**: 식사, 청소, 세탁 등 일상 지원 서비스 기록
- **응급 상황 대응**: 응급 상황 발생 시 신속한 기록 및 알림 체계 제공

---

## 🔑 시스템 주요 기능

1. **입소자 관리**
   - 입소자 정보(이름, 건강 기록, 보호자 정보 등) 저장 및 조회
2. **건강 관리**
   - 건강 데이터, 약물 투약 일정, 정기 검진 이력 관리
3. **직원 관리**
   - 직원의 역할, 일정, 배정 기록 관리
4. **생활 지원 서비스**
   - 식사, 청소, 세탁 등의 일상 지원 서비스 기록
5. **응급 상황 관리**
   - 응급 상황 발생 내역 및 보호자 알림 기록

---

## 📊 데이터베이스 설계

### 📝 개념적 설계
사용자 요구사항과 비즈니스 규칙을 기반으로 작성된 ER 다이어그램은 다음의 주요 엔티티와 관계를 포함합니다:
- **Resident** (입소자)
- **Guardian** (보호자)
- **HealthRecord** (건강 기록)
- **Medication** (약물)
- **Staff** (직원)
- **Emergency** (응급 상황)
- **LifeSupport** (생활 지원 서비스)

### 🛠️ 논리적 설계
데이터베이스는 **제3정규형(3NF)**을 준수하며, 주요 테이블은 다음과 같습니다:
- **Resident**: 입소자 정보 저장
- **HealthRecord**: 건강 데이터 및 약물 기록 관리
- **Staff**: 직원 정보 및 배정
- **Emergency**: 응급 상황 기록
- **LifeSupport**: 생활 지원 서비스 기록

### 💾 물리적 설계
모든 테이블은 기본 키, 외래 키, 제약 조건 등을 통해 데이터 무결성을 유지하도록 설계되었습니다.

---

## 🛠️ SQL 쿼리

프로젝트는 **10개 이상의 유용한 SQL 쿼리**를 포함하며, 주요 예시는 다음과 같습니다:
1. 특정 입소자의 최근 한 달간 건강 기록 조회
2. 특정 입소자를 관리하는 직원 정보 확인
3. 지난 30일간 발생한 응급 상황 목록 출력
4. 특정 입소자의 생활 지원 서비스 내역 조회
5. 다중 테이블을 활용한 조인 및 서브쿼리

---

## 📂 사용 방법

1. **데이터베이스 설정**
   - 제공된 SQL 스크립트를 사용하여 Oracle DBMS에 테이블을 생성하고 데이터를 삽입합니다.
2. **쿼리 실행**
   - 제공된 SQL 쿼리를 실행하여 데이터베이스의 기능을 확인합니다.
3. **데이터 탐색**
   - 필요에 따라 커스텀 쿼리를 작성하여 데이터 분석 및 관리 작업을 수행합니다.

---

## 📜 라이선스

이 프로젝트는 **"DB 설계 및 구현 2"** 과목의 학습 목적으로 수행된 프로젝트이며, 상업적 용도로 사용되지 않습니다.
