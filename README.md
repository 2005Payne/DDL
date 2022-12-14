# DDL_CREATE
## 테이블 생성
CREATE TABLE 테이블명(   
  필드이름 데이터타입 제약조건,   
  필드이름 데이터타입 제약조건,   
  필드이름 데이터타입 제약조건,   
  필드이름 데이터타입 제약조건   
);   

## 시퀀스 생성
CREATE SEQUENCE 시퀀스이름   
START WHIT 시작 값   
INCREMENT BY 증가 값   
MAXVALUE 최대 값   
MINVALUED 최소 값   
NOCYCLE(반복안함)/CYCLE(최대값 도달 시 최솟값 부터 시작)   
NOCACHE(사용안함)/CACHE(캐시를 사용하여 미리 값을 할당해 속도가 빠름)   
# DDL_ALTER
## 테이블 컬럼 추가
ALTER TABLE 테이블명 ADD(컬럼명 데이터타입(사이즈));
## 제약 조건 추가
ALTER TABLE 테이블명 ADD CONSTRAINT 제약조건명 제약조건(컬럼명);
## 테이블 컬럼 수정
ALTER TABLE 테이블명 MODIFY(컬럼명 데이터타입(사이즈));
## 테이블 컬럼 삭제하기
ALTER TABLE 테이블명 DROP COLUMN 컬럼명;
## 테이블 컬럼 이름 변경하기
ALTER TABLE 테이블명 RENAME COLUMN 컬럼명 TO 바꿀컬럼명;
# DDL_DROP
## 테이블 제거
DROP TABLE 테이블명;
## 시퀀스 제거
DROP SEQUENCE 시퀀스명;
