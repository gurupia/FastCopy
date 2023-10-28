# FastCopy

======================================================================  
FastCopy ver3.63 2019/02/19  
H. Shirouzu (시라미즈 히로아키)  
FastCopy Lab, LLC.  

한글번역: gurupia(파파고 번역 + 오탈자 수정)  
======================================================================    

특징:
Windows 계열에서 가장 빠른 파일 복사 & 삭제 도구입니다.

NT계열 OS 의 경우, UNICODE 로 밖에 표현할 수 없는 파일명이나 MAX_PATH(260글자)를  
넘는 위치의 파일도 카피(&삭제)할 수 있습니다.

자동으로 복사원본과 복사대상이 동일한 물리 저장장치별 저장장치(HDD,SSD,FlashMemory)인지 판정후  
이하의 동작을 실시합니다.

다른 물리적 저장장치간 멀티 스레드에서 읽기와 쓰기를 병렬로 실행합니다.

동일 물리적 저장장치의 복사원본에서 (버퍼가 가득 찰 때까지) 연속 읽기 후,
복사대상에 연속해서 써넣습니다

Read/Write도 OS 캐시를 전혀 사용하지 않기 때문에 다른 프로세스로 동작 합니다.
(애플리케이션)이 무거워지기 어렵게 되어 있습니다.

가능한 한 큰 단위로 Read/Write 하기 때문에 디바이스의 한계에 가까운 퍼포먼스가 나옵니다.


Include/Exclude 필터(UNIX 와일드 카드 형식)가 지정 가능합니다.

MFC 등의 프레임워크를 사용하지 않고 Win32API만으로 만들고 있으므로,
경량 & 콤팩트 & 빠르게 작동합니다.

라이선스입니다.
FastCopy ver3.x
Copyright(C) 2004-2019 SHIROUZU Hiroaki All rights reserved.
Copyright(C) 2018-2019 FastCopy Lab, LLC. All rights reserved.

전체 소스 코드는 GPLv3에서 공개하고 있습니다.
VC++ 등을 가지고 계신다면 커스터마이즈 이용도 가능합니다.
자세한 내용은 동봉된 license-gpl3.txt를 참조하십시오.

xxHash library
Copyright (C) 2012-2016 Mr.Yann Collet, All rights reserved.
more details: external/xxhash/LICENSE

사용법은 도움말(fastcopy.htm)을 참조하십시오.

소스 빌드 환경은 VS2017 이후로 빌드할 수 있습니다.
