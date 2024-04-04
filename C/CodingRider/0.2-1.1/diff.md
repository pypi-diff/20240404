# Comparing `tmp/CodingRider-0.2.tar.gz` & `tmp/CodingRider-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodingRider-0.2.tar", last modified: Wed Nov 15 03:17:07 2023, max compression
+gzip compressed data, was "CodingRider-1.1.tar", last modified: Thu Apr  4 04:14:28 2024, max compression
```

## Comparing `CodingRider-0.2.tar` & `CodingRider-1.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 03:17:07.871605 CodingRider-0.2/
-drwxrwxrwx   0        0        0        0 2023-11-15 03:17:07.826617 CodingRider-0.2/CodingRider/
--rw-rw-rw-   0        0        0      109 2023-03-28 08:35:12.000000 CodingRider-0.2/CodingRider/__init__.py
--rw-rw-rw-   0        0        0      737 2023-11-15 01:18:44.000000 CodingRider-0.2/CodingRider/__main__.py
--rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-0.2/CodingRider/crc.py
--rw-rw-rw-   0        0        0    50210 2023-11-15 01:22:08.000000 CodingRider-0.2/CodingRider/drone.py
--rw-rw-rw-   0        0        0    77888 2023-11-15 01:18:49.000000 CodingRider-0.2/CodingRider/protocol.py
--rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-0.2/CodingRider/receiver.py
--rw-rw-rw-   0        0        0     2482 2023-11-15 01:18:50.000000 CodingRider-0.2/CodingRider/storage.py
--rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-0.2/CodingRider/system.py
--rw-rw-rw-   0        0        0     9515 2023-11-15 01:18:52.000000 CodingRider-0.2/CodingRider/update.py
-drwxrwxrwx   0        0        0        0 2023-11-15 03:17:07.867770 CodingRider-0.2/CodingRider.egg-info/
--rw-rw-rw-   0        0        0      626 2023-11-15 03:17:07.000000 CodingRider-0.2/CodingRider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-11-15 03:17:07.000000 CodingRider-0.2/CodingRider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 03:17:07.000000 CodingRider-0.2/CodingRider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-11-15 03:17:07.000000 CodingRider-0.2/CodingRider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-11-15 03:17:07.000000 CodingRider-0.2/CodingRider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-0.2/LICENSE
--rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2023-11-15 03:17:07.870552 CodingRider-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-11-15 03:17:07.871605 CodingRider-0.2/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-11-15 03:12:42.000000 CodingRider-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.606468 CodingRider-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.589754 CodingRider-1.1/CodingRider/
+-rw-rw-rw-   0        0        0      109 2024-04-04 04:14:10.000000 CodingRider-1.1/CodingRider/__init__.py
+-rw-rw-rw-   0        0        0      484 2023-12-25 23:04:18.000000 CodingRider-1.1/CodingRider/__main__.py
+-rw-rw-rw-   0        0        0     4609 2023-03-28 08:35:12.000000 CodingRider-1.1/CodingRider/crc.py
+-rw-rw-rw-   0        0        0    43609 2024-03-28 06:44:10.000000 CodingRider-1.1/CodingRider/drone.py
+-rw-rw-rw-   0        0        0    70379 2024-04-04 03:58:07.000000 CodingRider-1.1/CodingRider/protocol.py
+-rw-rw-rw-   0        0        0     7088 2023-11-15 01:18:50.000000 CodingRider-1.1/CodingRider/receiver.py
+-rw-rw-rw-   0        0        0     1904 2023-12-25 23:03:04.000000 CodingRider-1.1/CodingRider/storage.py
+-rw-rw-rw-   0        0        0    10249 2023-03-28 08:35:12.000000 CodingRider-1.1/CodingRider/system.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:14:28.604434 CodingRider-1.1/CodingRider.egg-info/
+-rw-rw-rw-   0        0        0      626 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 04:14:28.000000 CodingRider-1.1/CodingRider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-03-28 08:35:12.000000 CodingRider-1.1/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-03-28 08:35:12.000000 CodingRider-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2024-04-04 04:14:28.605470 CodingRider-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-11-15 03:15:25.000000 CodingRider-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 04:14:28.606468 CodingRider-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      778 2024-04-04 04:06:45.000000 CodingRider-1.1/setup.py
```

### Comparing `CodingRider-0.2/CodingRider/crc.py` & `CodingRider-1.1/CodingRider/crc.py`

 * *Files identical despite different names*

### Comparing `CodingRider-0.2/CodingRider/drone.py` & `CodingRider-1.1/CodingRider/drone.py`

 * *Files 10% similar despite different names*

```diff
@@ -499,44 +499,40 @@
 
         data.dataType   = dataType
 
         return self.transfer(header, data)
 
 
 
-    def sendPairing(self, deviceType, address0, address1, address2, scramble, channel0, channel1, channel2, channel3):
+    def sendPairing(self, deviceType, address0, address1, address2, address3, address4, channel0):
     
         if  ( (not isinstance(deviceType, DeviceType)) or
             (not isinstance(address0, int)) or
             (not isinstance(address1, int)) or
             (not isinstance(address2, int)) or
-            (not isinstance(scramble, int)) or
-            (not isinstance(channel0, int)) or
-            (not isinstance(channel1, int)) or
-            (not isinstance(channel2, int)) or
-            (not isinstance(channel3, int)) ):
+            (not isinstance(address3, int)) or
+            (not isinstance(address4, int)) or
+            (not isinstance(channel0, int)) ):
             return None
 
         header = Header()
         
         header.dataType = DataType.Pairing
         header.length   = Pairing.getSize()
         header.from_    = DeviceType.Base
         header.to_      = deviceType
 
         data = Pairing()
 
         data.address0   = address0
         data.address1   = address1
         data.address2   = address2
-        data.scramble   = scramble
+        data.address3   = address3
+        data.address4   = address4
         data.channel0   = channel0
-        data.channel1   = channel1
-        data.channel2   = channel2
-        data.channel3   = channel3
 
         return self.transfer(header, data)
 
 
 # Common Start
 
 
@@ -1304,231 +1300,14 @@
 
 
 
 # Light End
 
 
 
-# Display Start
-
-
-    def sendDisplayClearAll(self, pixel = DisplayPixel.Black):
-        
-        if ( not isinstance(pixel, DisplayPixel) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayClear
-        header.length   = DisplayClearAll.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayClearAll()
-
-        data.pixel      = pixel
-
-        return self.transfer(header, data)
-    
-
-
-    def sendDisplayClear(self, x, y, width, height, pixel = DisplayPixel.Black):
-        
-        if ( not isinstance(pixel, DisplayPixel) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayClear
-        header.length   = DisplayClear.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayClear()
-
-        data.x          = x
-        data.y          = y
-        data.width      = width
-        data.height     = height
-        data.pixel      = pixel
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayInvert(self, x, y, width, height):
-        
-        header = Header()
-        
-        header.dataType = DataType.DisplayInvert
-        header.length   = DisplayInvert.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayInvert()
-
-        data.x          = x
-        data.y          = y
-        data.width      = width
-        data.height     = height
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawPoint(self, x, y, pixel = DisplayPixel.White):
-        
-        if ( not isinstance(pixel, DisplayPixel) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawPoint
-        header.length   = DisplayDrawPoint.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawPoint()
-
-        data.x          = x
-        data.y          = y
-        data.pixel      = pixel
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawLine(self, x1, y1, x2, y2, pixel = DisplayPixel.White, line = DisplayLine.Solid):
-        
-        if ( (not isinstance(pixel, DisplayPixel)) or (not isinstance(line, DisplayLine)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawLine
-        header.length   = DisplayDrawLine.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawLine()
-
-        data.x1         = x1
-        data.y1         = y1
-        data.x2         = x2
-        data.y2         = y2
-        data.pixel      = pixel
-        data.line       = line
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawRect(self, x, y, width, height, pixel = DisplayPixel.White, flagFill = False, line = DisplayLine.Solid):
-        
-        if ( (not isinstance(pixel, DisplayPixel)) or (not isinstance(flagFill, bool)) or (not isinstance(line, DisplayLine)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawRect
-        header.length   = DisplayDrawRect.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawRect()
-
-        data.x          = x
-        data.y          = y
-        data.width      = width
-        data.height     = height
-        data.pixel      = pixel
-        data.flagFill   = flagFill
-        data.line       = line
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawCircle(self, x, y, radius, pixel = DisplayPixel.White, flagFill = True):
-        
-        if ( (not isinstance(pixel, DisplayPixel)) or (not isinstance(flagFill, bool)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawCircle
-        header.length   = DisplayDrawCircle.getSize()
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawCircle()
-
-        data.x          = x
-        data.y          = y
-        data.radius     = radius
-        data.pixel      = pixel
-        data.flagFill   = flagFill
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawString(self, x, y, message, font = DisplayFont.LiberationMono5x8, pixel = DisplayPixel.White):
-        
-        if ( (not isinstance(font, DisplayFont)) or (not isinstance(pixel, DisplayPixel)) or (not isinstance(message, str)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawString
-        header.length   = DisplayDrawString.getSize() + len(message)
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawString()
-
-        data.x          = x
-        data.y          = y
-        data.font       = font
-        data.pixel      = pixel
-        data.message    = message
-
-        return self.transfer(header, data)
-
-
-
-    def sendDisplayDrawStringAlign(self, x_start, x_end, y, message, align = DisplayAlign.Center, font = DisplayFont.LiberationMono5x8, pixel = DisplayPixel.White):
-        
-        if ( (not isinstance(align, DisplayAlign)) or (not isinstance(font, DisplayFont)) or (not isinstance(pixel, DisplayPixel)) or (not isinstance(message, str)) ):
-            return None
-
-        header = Header()
-        
-        header.dataType = DataType.DisplayDrawStringAlign
-        header.length   = DisplayDrawStringAlign.getSize() + len(message)
-        header.from_    = DeviceType.Base
-        header.to_      = DeviceType.Controller
-        
-        data = DisplayDrawStringAlign()
-
-        data.x_start    = x_start
-        data.x_end      = x_end
-        data.y          = y
-        data.align      = align
-        data.font       = font
-        data.pixel      = pixel
-        data.message    = message
-
-        return self.transfer(header, data)
-
-
-# Display End
-
-
-
 # Buzzer Start
 
 
     def sendBuzzer(self, mode, value, time):
         
         if ( (not isinstance(mode, BuzzerMode)) or (not isinstance(value, int)) or (not isinstance(time, int)) ):
             return None
```

### Comparing `CodingRider-0.2/CodingRider/protocol.py` & `CodingRider-1.1/CodingRider/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,101 +37,54 @@
     Ping                        = 0x01      # 통신 확인
     Ack                         = 0x02      # 데이터 수신에 대한 응답
     Error                       = 0x03      # 오류(reserve, 비트 플래그는 추후에 지정)
     Request                     = 0x04      # 지정한 타입의 데이터 요청
     Message                     = 0x05      # 문자열 데이터
     Address                     = 0x06      # 장치 주소(MAC이 있는 경우 MAC) 혹은 고유번호(MAC이 없는 경우 UUID)
     Information                 = 0x07      # 펌웨어 및 장치 정보
-    Update                      = 0x08      # 펌웨어 업데이트
-    UpdateLocation              = 0x09      # 펌웨어 업데이트 위치 정정
-    Encrypt                     = 0x0A      # 펌웨어 암호화
-    SystemCount                 = 0x0B      # 시스템 카운트
-    SystemInformation           = 0x0C      # 시스템 정보
-    Registration                = 0x0D      # 제품 등록
-    Administrator               = 0x0E      # 관리자 권한 획득
-    Monitor                     = 0x0F      # 디버깅용 값 배열 전송. 첫번째 바이트에 타입, 두 번째 바이트에 페이지 지정(수신 받는 데이터의 저장 경로 구분)
     Control                     = 0x10      # 조종
 
     Command                     = 0x11      # 명령
     Pairing                     = 0x12      # 페어링
     Rssi                        = 0x13      # RSSI
-    TimeSync                    = 0x14      # 시간 동기화
-    TransmissionPower           = 0x15      # 전송 출력
-    Configuration               = 0x16      # 설정
     
     Battle                      = 0x1F      # 전투
 
     # Light
     LightManual                 = 0x20      # LED 수동 제어
     LightMode                   = 0x21      # LED 모드
     LightEvent                  = 0x22      # LED 이벤트
     LightDefault                = 0x23      # LED 초기 모드
 
     # 센서 RAW 데이터
     RawMotion                   = 0x30      # Motion 센서 데이터 RAW 값
-    RawFlow                     = 0x31      # Flow 센서 데이터 RAW 값
 
     # 상태, 센서
     State                       = 0x40      # 드론의 상태(비행 모드 방위기준 배터리량)
-    Attitude                    = 0x41      # 드론의 자세(Angle)
-    Position                    = 0x42      # 위치
     Altitude                    = 0x43      # 높이, 고도
     Motion                      = 0x44      # Motion 센서 데이터 처리한 값(IMU)
-    Range                       = 0x45      # 거리센서 데이터
+    VisionSensor				= 0x47,		# Vision Sensor X, Y, Z
 
     # 설정
     Count                       = 0x50      # 카운트
-    Bias                        = 0x51      # 엑셀, 자이로 바이어스 값
     Trim                        = 0x52      # 트림
-    Weight                      = 0x53      # 무게
     LostConnection              = 0x54      # 연결이 끊긴 후 반응 시간 설정
 
     # Devices
-    Motor                       = 0x60      # 모터 제어 및 현재 제어값 확인
-    MotorSingle                 = 0x61      # 한 개의 모터 제어
     Buzzer                      = 0x62      # 부저 제어
     Vibrator                    = 0x63      # 진동 제어
+    Battery					    = 0x64,		# 배터리
 
     # Input
     Button                      = 0x70      # 버튼 입력
     Joystick                    = 0x71      # 조이스틱 입력
-
-    # Display
-    DisplayClear                = 0x80      # 화면 지우기
-    DisplayInvert               = 0x81      # 화면 반전
-    DisplayDrawPoint            = 0x82      # 점 그리기
-    DisplayDrawLine             = 0x83      # 선 그리기
-    DisplayDrawRect             = 0x84      # 사각형 그리기
-    DisplayDrawCircle           = 0x85      # 원 그리기
-    DisplayDrawString           = 0x86      # 문자열 쓰기
-    DisplayDrawStringAlign      = 0x87      # 문자열 쓰기
-    DisplayDrawImage            = 0x88      # 그림 그리기
-
-    # Card
-    CardClassify                = 0x90      # 카드 색상 분류 기준 설정
-    CardRange                   = 0x91      # 카드 색 범위(RAW 데이터의 출력 범위)
-    CardRaw                     = 0x92      # 카드 데이터 RAW 값(유선으로만 전송)
-    CardColor                   = 0x93      # 카드 데이터
-    CardList                    = 0x94      # 카드 리스트 데이터
-    CardFunctionList            = 0x95      # 카드 함수 리스트 데이터
     
     # Information Assembled
     InformationAssembledForController   = 0xA0      # 자주 갱신되는 데이터 모음
     InformationAssembledForEntry        = 0xA1      # 자주 갱신되는 데이터 모음
-    InformationAssembledForByBlocks     = 0xA2      # 자주 갱신되는 데이터 모음
-
-    # Navigation
-    NavigationTarget                    = 0xD0      # 네비게이션 목표점
-    NavigationLocation                  = 0xD1      # 네비게이션 가상 위치
-    NavigationMonitor                   = 0xD2
-    NavigationHeading                   = 0xD3
-    NavigationCounter                   = 0xD4
-
-    GpsRtkNavigationState               = 0xDA      # RTK RAW 데이터 전송
-    GpsRtkExtendedRawMeasurementData    = 0xDB      # RTK RAW 데이터 전송
 
     EndOfType                           = 0xDC
 
 
 # DataType End
 
 
@@ -152,33 +105,19 @@
 
     ClearBias               = 0x05      # 자이로 바이어스 리셋(트림도 같이 초기화 됨)
     ClearTrim               = 0x06      # 트림 초기화
 
     FlightEvent             = 0x07      # 비행 이벤트 실행
 
     SetDefault              = 0x08      # 기본 설정으로 초기화
-    Backlight               = 0x09      # 조종기 백라이트 설정
     ModeController          = 0x0A      # 조종기 동작 모드(0x10:조종, 0x80:링크)
     Link                    = 0x0B      # 링크 제어(0:Client Mode, 1:Server Mode, 2:Pairing Start)
 
-    # 관리자
-    ClearCounter            = 0xA0      # 카운터 클리어(관리자 권한을 획득했을 경우에만 동작)
-
-    # Navigation
-    NavigationTargetClear   = 0xE0      # 네비게이션 목표점 초기화
-    NavigationStart         = 0xE1      # 네비게이션 시작(처음부터)
-    NavigationPause         = 0xE2      # 네비게이션 일시 정지
-    NavigationRestart       = 0xE3      # 네비게이션 다시 시작(일시 정지 후 다시 시작할 때 사용)
-    NavigationStop          = 0xE4      # 네비게이션 중단
-    NavigationNext          = 0xE5      # 네비게이션 목표점을 다음으로 변경
-    NavigationReturnToHome  = 0xE6      # 시작 위치로 귀환
+    ModeTest				= 0xF0      # 테스트 모드
     
-    GpsRtkBase              = 0xEA
-    GpsRtkRover             = 0xEB
-
     EndOfType               = 0xEC
 
 
 # CommandType End
 
 
 
@@ -566,79 +505,42 @@
             return None
         
         data.address = dataArray[0:16]
         return data
 
 
 
-class RegistrationInformation(ISerializable):
-
-    def __init__(self):
-        self.address        = bytearray()
-        self.year           = 0
-        self.month          = 0
-        self.key            = 0
-        self.flagValid      = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 21
-
-
-    def toArray(self):
-        dataArray = bytearray()
-        dataArray.extend(self.address)
-        dataArray.extend(pack('<HBB?', self.year, self.month, self.key, self.flagValid))
-        return dataArray
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = RegistrationInformation()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.address = dataArray[0:16]
-        data.year, data.month, data.key, data.flagValid = unpack('<HBB?', dataArray[16:21])
-        return data
-
-
-
 class Pairing(ISerializable):
 
     def __init__(self):
         self.address0       = 0
         self.address1       = 0
         self.address2       = 0
-        self.scramble       = 0
+        self.address3       = 0
+        self.address4       = 0
         self.channel0       = 0
-        self.channel1       = 0
-        self.channel2       = 0
-        self.channel3       = 0
 
 
     @classmethod
     def getSize(cls):
         return 11
 
 
     def toArray(self):
-        return pack('<HHHBBBBB', self.address0, self.address1, self.address2, self.scramble, self.channel0, self.channel1, self.channel2, self.channel3)
+        return pack('<BBBBBB', self.address0, self.address1, self.address2, self.address3, self.address4, self.channel0)
 
 
     @classmethod
     def parse(cls, dataArray):
         data = Pairing()
         
         if len(dataArray) != cls.getSize():
             return None
         
-        data.address0, data.address1, data.address2, data.scramble, data.channel0, data.channel1, data.channel2, data.channel3 = unpack('<HHHBBBBB', dataArray)
+        data.address0, data.address1, data.address2, data.address3, data.address4, data.channel0 = unpack('<BBBBBB', dataArray)
         return data
 
 
 
 class Rssi(ISerializable):
 
     def __init__(self):
@@ -803,172 +705,14 @@
         return data
 
 
 # Common End
 
 
 
-# Monitor Start
-
-
-class MonitorHeaderType(Enum):
-    
-    Monitor0            = 0x00
-    Monitor4            = 0x01
-    Monitor8            = 0x02
-
-    EndOfType           = 0x03
-
-
-
-class MonitorDataType(Enum):
-    
-    U8          = 0x00,
-    S8          = 0x01,
-    U16         = 0x02,
-    S16         = 0x03,
-    U32         = 0x04,
-    S32         = 0x05,
-    U64         = 0x06,
-    S64         = 0x07,
-    F32         = 0x08,
-    F64         = 0x09,
-
-    EndOfType   = 0x0A
-
-
-
-class MonitorType(ISerializable):
-
-    def __init__(self):
-        self.monitorHeaderType    = MonitorHeaderType.Monitor8
-
-
-    @classmethod
-    def getSize(cls):
-        return 1
-
-
-    def toArray(self):
-        return pack('<B', self.monitorHeaderType.value)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = MonitorType()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.monitorHeaderType, = unpack('<B', dataArray)
-
-        data.monitorHeaderType  = MonitorHeaderType(data.monitorHeaderType)
-
-        return data
-
-
-
-class Monitor0(ISerializable):
-
-    def __init__(self):
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 2
-
-
-    def toArray(self):
-        return pack('<BB', self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor0()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.monitorDataType, data.index = unpack('<BB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-class Monitor4(ISerializable):
-
-    def __init__(self):
-        self.systemTime             = 0
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 6
-
-
-    def toArray(self):
-        return pack('<IBB', self.systemTime, self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor4()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.systemTime, data.monitorDataType, data.index = unpack('<IBB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-class Monitor8(ISerializable):
-    
-    def __init__(self):
-        self.systemTime             = 0
-        self.monitorDataType        = MonitorDataType.F32
-        self.index                  = 0
-
-
-    @classmethod
-    def getSize(cls):
-        return 10
-
-
-    def toArray(self):
-        return pack('<QBB', self.systemTime, self.monitorDataType.value, self.index)
-
-
-    @classmethod
-    def parse(cls, dataArray):
-        data = Monitor8()
-        
-        if len(dataArray) != cls.getSize():
-            return None
-        
-        data.systemTime, data.monitorDataType, data.index = unpack('<QBB', dataArray)
-
-        data.monitorDataType  = MonitorDataType(data.monitorDataType)
-
-        return data
-
-
-
-# Monitor End
-
-
 
 # Control Start
 
 
 class ControlQuad8(ISerializable):
 
     def __init__(self):
@@ -1106,112 +850,126 @@
 
 # Light Start
 
 
 class LightModeDrone(Enum):
     
     None_                   = 0x00
-
-    RearNone                = 0x10
-    RearManual              = 0x11      # 수동 제어
-    RearHold                = 0x12      # 지정한 색상을 계속 켬
-    RearFlicker             = 0x13      # 깜빡임
-    RearFlickerDouble       = 0x14      # 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)
-    RearDimming             = 0x15      # 밝기 제어하여 천천히 깜빡임
-    RearSunrise             = 0x16
-    RearSunset              = 0x17
-
-    BodyNone                = 0x20
-    BodyManual              = 0x21      # 수동 제어
-    BodyHold                = 0x22      # 지정한 색상을 계속 켬
-    BodyFlicker             = 0x23      # 깜빡임
-    BodyFlickerDouble       = 0x24      # 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)
-    BodyDimming             = 0x25      # 밝기 제어하여 천천히 깜빡임
-    BodySunrise             = 0x26
-    BodySunset              = 0x27
-    BodyRainbow             = 0x28
-    BodyRainbow2            = 0x29
-
-    ANone                   = 0x30
-    AManual                 = 0x31      # 수동 제어
-    AHold                   = 0x32      # 지정한 색상을 계속 켬
-    AFlicker                = 0x33      # 깜빡임
-    AFlickerDouble          = 0x34      # 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)
-    ADimming                = 0x35      # 밝기 제어하여 천천히 깜빡임
-    ASunrise                = 0x36
-    ASunset                 = 0x37
-
-    BNone                   = 0x40
-    BManual                 = 0x41      # 수동 제어
-    BHold                   = 0x42      # 지정한 색상을 계속 켬
-    BFlicker                = 0x43      # 깜빡임
-    BFlickerDouble          = 0x44      # 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)
-    BDimming                = 0x45      # 밝기 제어하여 천천히 깜빡임
-    BSunrise                = 0x46
-    BSunset                 = 0x47
-
-    CNone                   = 0x50
-    CManual                 = 0x51      # 수동 제어
-    CHold                   = 0x52      # 지정한 색상을 계속 켬
-    CFlicker                = 0x53      # 깜빡임
-    CFlickerDouble          = 0x54      # 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)
-    CDimming                = 0x55      # 밝기 제어하여 천천히 깜빡임
-    CSunrise                = 0x56
-    CSunset                 = 0x57
-    CRainbow                = 0x58
-    CRainbow2               = 0x59
-
+    
+    # Team (Forward, Rear를 동시에 제어)
+    TeamRgbNone				= 0x10
+    TeamRgbManual			= 0x11		# 수동 제어
+    TeamRgbHold				= 0x12		# 지정한 색상을 계속 켬
+    TeamRgbFlicker			= 0x13		# 깜빡임			
+    TeamRgbFlickerDouble	= 0x14		# 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)			
+    TeamRgbDimming			= 0x15		# 밝기 제어하여 천천히 깜빡임
+    TeamRgbSunrise			= 0x16		# 꺼진 상태에서 점점 밝아짐
+    TeamRgbSunset			= 0x17		# 켜진 상태에서 점점 어두워짐
+    TeamRgbRainbow			= 0x18		# 무지개색
+    TeamRgbRainbow2			= 0x19		# 무지개색
+    TeamRgbRedBlue			= 0x1A		# Red-Blue
+    
+    TeamFlowForward			= 0x1E		# 앞으로 흐름 
+    TeamWarning				= 0x1F		# 경고
+    
+    # Body
+    BodyNone				= 0x20		
+    BodyManual				= 0x21		# 수동 제어
+    BodyHold				= 0x22		# 지정한 색상을 계속 켬
+    BodyFlicker				= 0x23		# 깜빡임			
+    BodyFlickerDouble		= 0x24		# 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)			
+    BodyDimming				= 0x25		# 밝기 제어하여 천천히 깜빡임
+    BodySunrise				= 0x26		# 꺼진 상태에서 점점 밝아짐
+    BodySunset				= 0x27		# 켜진 상태에서 점점 어두워짐
+    BodyRainbow				= 0x28		# 무지개색
+    BodyRainbow2			= 0x29		# 무지개색
+    BodyRedBlue				= 0x2A		# Red-Blue
+    BodyCard				= 0x2B		# 카드 색상 표시(이벤트용)
+    BodyWarning				= 0x2F		# 경고
+    
+    # Link
+    LinkNone				= 0x30		
+    LinkManual				= 0x31		# 수동 제어
+    LinkHold				= 0x32		# 지정한 색상을 계속 켬
+    LinkFlicker				= 0x33		# 깜빡임			
+    LinkFlickerDouble		= 0x34		# 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)			
+    LinkDimming				= 0x35		# 밝기 제어하여 천천히 깜빡임
+    LinkSunrise				= 0x36		# 꺼진 상태에서 점점 밝아짐
+    LinkSunset				= 0x37		# 켜진 상태에서 점점 어두워짐
+    
     EndOfType               = 0x60
 
 
 
 class LightFlagsDrone(Enum):
     
-    None_               = 0x0000
-
-    Rear                = 0x0001
-    BodyRed             = 0x0002
-    BodyGreen           = 0x0004
-    BodyBlue            = 0x0008
-
-    A                   = 0x0010
-    B                   = 0x0020
-    CRed                = 0x0040
-    CGreen              = 0x0080
-    CBlue               = 0x0100
+    None_			= 0x0000
+    
+    BodyRed			= 0x0001
+    BodyGreen		= 0x0002
+    BodyBlue		= 0x0004
+    
+    TeamRed			= 0x0008
+    TeamBlue		= 0x0010
+    
+    Link			= 0x0080
 
 
 
 class LightModeController(Enum):
     
-    None_               = 0x00
-
-    # Body
-    BodyNone            = 0x20
-    BodyManual          = 0x21      # 수동 조작
-    BodyHold            = 0x22
-    BodyFlicker         = 0x23
-    BodyFlickerDouble   = 0x24
-    BodyDimming         = 0x25
-    BodySunrise         = 0x26
-    BodySunset          = 0x27
-    BodyRainbow         = 0x28
-    BodyRainbow2        = 0x29
-
-    EndOfType           = 0x30
+    # Team
+    TeamNone						= 0x10
+    TeamManual						= 0x11		# 수동 제어
+    TeamHold						= 0x12		# 지정한 색상을 계속 켬
+    TeamFlicker						= 0x13		# 깜빡임			
+    TeamFlickerDouble				= 0x14		# 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)			
+    TeamDimming						= 0x15		# 밝기 제어하여 천천히 깜빡임
+    TeamSunrise						= 0x16		# 꺼진 상태에서 점점 밝아짐
+    TeamSunset						= 0x17		# 켜진 상태에서 점점 어두워짐
+    TeamRedBlue						= 0x1A		# Red-Blue
+    
+    # Array 6
+    Array6None						= 0x30
+    Array6Manual					= 0x31		# 수동 제어
+    Array6Hold						= 0x32		# [전체] 지정한 색상을 계속 켬
+    Array6Flicker					= 0x33		# [전체] 깜빡임			
+    Array6FlickerDouble				= 0x34		# [전체] 깜빡임(두 번 깜빡이고 깜빡인 시간만큼 꺼짐)		
+    Array6Dimming					= 0x35		# [전체] 밝기 제어하여 천천히 깜빡임
+    
+    # Array 6 Value
+    Array6ValueNone					= 0x40		# [개별] 0 ~ 255 사이의 값 표시
+    Array6ValueHold					= 0x42		# [개별] 0 ~ 255 사이의 값 표시
+    Array6ValueFlicker				= 0x43		# [개별] 0 ~ 255 사이의 값 표시
+    Array6ValueFlickerDouble		= 0x44		# [개별] 0 ~ 255 사이의 값 표시
+    Array6ValueDimming				= 0x45		# [개별] 0 ~ 255 사이의 값 표시
+    
+    # Array 6 Function
+    Array6FunctionNone				= 0x50
+    Array6Pendulum					= 0x51
+    Array6FlowLeft					= 0x52		# [개별] 왼쪽으로 흐름
+    Array6FlowRight					= 0x53		# [개별] 오른쪽으로 흐름
+    
+    EndOfType                       = 0x60
 
 
 
 class LightFlagsController(Enum):
     
-    None_               = 0x00
+    None_               = 0x0000
 
-    BodyRed             = 0x01
-    BodyGreen           = 0x02
-    BodyBlue            = 0x04
+    TeamRed		        = 0x0001
+    TeamBlue	        = 0x0002
+            
+    E0			        = 0x0004
+    E1			        = 0x0008
+    E2			        = 0x0010
+    E3			        = 0x0020
+    E4			        = 0x0040
+    E5			        = 0x0080
 
 
 
 class Color(ISerializable):
 
     def __init__(self):
         self.r      = 0
```

### Comparing `CodingRider-0.2/CodingRider/receiver.py` & `CodingRider-1.1/CodingRider/receiver.py`

 * *Files identical despite different names*

### Comparing `CodingRider-0.2/CodingRider/storage.py` & `CodingRider-1.1/CodingRider/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,35 +47,26 @@
 
         self.d[DataType.Ping]               = Ping.parse
         self.d[DataType.Ack]                = Ack.parse
         self.d[DataType.Error]              = Error.parse
         self.d[DataType.Message]            = Message.parse
         self.d[DataType.Address]            = Address.parse
         self.d[DataType.Information]        = Information.parse
-        self.d[DataType.UpdateLocation]     = UpdateLocation.parse
-        self.d[DataType.SystemInformation]  = SystemInformation.parse
-        self.d[DataType.Registration]       = RegistrationInformation.parse
 
         self.d[DataType.Pairing]            = Pairing.parse
         self.d[DataType.Rssi]               = Rssi.parse
 
         self.d[DataType.RawMotion]          = RawMotion.parse
-        self.d[DataType.RawFlow]            = RawFlow.parse
 
         self.d[DataType.State]              = State.parse
-        self.d[DataType.Attitude]           = Attitude.parse
-        self.d[DataType.Position]           = Position.parse
         self.d[DataType.Altitude]           = Altitude.parse
         self.d[DataType.Motion]             = Motion.parse
-        self.d[DataType.Range]              = Range.parse
 
         self.d[DataType.Count]              = Count.parse
-        self.d[DataType.Bias]               = Bias.parse
         self.d[DataType.Trim]               = Trim.parse
-        self.d[DataType.Weight]             = Weight.parse
 
         self.d[DataType.Button]             = Button.parse
         self.d[DataType.Joystick]           = Joystick.parse
 
         self.d[DataType.InformationAssembledForController]  = InformationAssembledForController.parse
         self.d[DataType.InformationAssembledForEntry]       = InformationAssembledForEntry.parse
```

### Comparing `CodingRider-0.2/CodingRider/system.py` & `CodingRider-1.1/CodingRider/system.py`

 * *Files identical despite different names*

### Comparing `CodingRider-0.2/CodingRider.egg-info/PKG-INFO` & `CodingRider-1.1/CodingRider.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 0.2
+Version: 1.1
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-0.2/PKG-INFO` & `CodingRider-1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodingRider
-Version: 0.2
+Version: 1.1
 Summary: Library for CodingRider
 Home-page: https://imssam.me/shop/view.php?index_no=4031
 Author: ALUX
 Author-email: devdrone@aluxonline.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CodingRider-0.2/setup.py` & `CodingRider-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # http://swdeveloper.tistory.com/34
 # https://code.tutsplus.com/ko/tutorials/how-to-share-your-python-packages--cms-26114
 # https://code.tutsplus.com/ko/tutorials/how-to-write-your-own-python-packages--cms-26076
 from setuptools import setup, find_packages
 
 setup(
     name = "CodingRider",
-    version = "0.2",
+    version = "1.1",
     description = "Library for CodingRider",
     author = "ALUX",
     author_email = "devdrone@aluxonline.com",
     url = "https://imssam.me/shop/view.php?index_no=4031",
     packages = find_packages(exclude=['tests']),
     install_requires = [
         'pyserial>=3.4',
         'numpy>=1.15.4',
         'colorama>=0.4.0'],
     long_description = open('README.md').read(),
     long_description_content_type='text/markdown',
 )
+
+
+
```

