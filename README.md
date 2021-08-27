# Barcode Xpress for .NET Samples

A set of minimal [Barcode Xpress for .NET](https://www.nuget.org/packages/Accusoft.BarcodeXpress.Net/)
applications written for C# and VB.NET. Each language has the following samples:

* read-barcodes - Demonstrates how to read barcodes from an image.
* write-barcodes-1d - Demonstrates how to generate a 1D Code 39 Barcode.
* write-barcodes-2d - Demonstrates how to generate a 2D DataMatrix Barcode.

## Requirements

Visual Studio 2012-2019 to build the samples.

For the full list of requirements to run the sample,
refer to the [Barcode Xpress for .NET help](https://help.accusoft.com/BarcodeXpress/latest/BxNet/webframe.html#System_Requirements.html).

## Running the Sample

First, open one of the solution files (Files ending in .sln) in Visual Studio
and build it. This will also restore required the NuGet packages.

Then, open the Command Prompt window, change the directory to the sample
location, and start the app:

    .\bin\Debug\ReadBarcodes.exe

For the reader samples you should see output like this:

    Results:
    [
      {
        "Area": "496, 81, 646, 99",
        "Point1": "496, 81",
        "Point2": "1142, 82",
        "Point3": "1142, 180",
        "Point4": "496, 180",
        "Skew": 0,
        "Confidence": 100,
        "ValidCheckSum": true,
        "NumberCheckSumChars": 0,
        "Length": 45,
        "BarcodeValue": "441231234561234567** UNLICENSED accusoft.com",
        "BarcodeData": [
          "4",
          "4",
          "1",
          "2",
          "3",
          "1",
          "2",
          "3",
          "4",
          "5",
          "6",
          "1",
          "2",
          "3",
          "4",
          "5",
          "6",
          "7",
          "*",
          "*",
          " ",
          "U",
          "N",
          "L",
          "I",
          "C",
          "E",
          "N",
          "S",
          "E",
          "D",
          " ",
          "a",
          "c",
          "c",
          "u",
          "s",
          "o",
          "f",
          "t",
          ".",
          "c",
          "o",
          "m",
          "\u0000"
        ],
        "BarcodeDataAsByte": "NDQxMjMxMjM0NTYxMjM0NTY3KiogVU5MSUNFTlNFRCBhY2N1c29mdC5jb20A",
        "BarcodeName": "IntelligentMail",
        "BarcodeType": 27,
        "ModeTransitions": [],
        "Info2D": {
          "RowsDetected": 0,
          "ColumnsDetected": 0,
          "Rows": 0,
          "Columns": 0,
          "ErrorCorrectionLevel": 0
        }
      },
      {
        "Area": "60, 89, 349, 84",
        "Point1": "60, 89",
        "Point2": "409, 89",
        "Point3": "409, 173",
        "Point4": "60, 173",
        "Skew": 0,
        "Confidence": 100,
        "ValidCheckSum": false,
        "NumberCheckSumChars": 0,
        "Length": 32,
        "BarcodeValue": "CODE ** UNLICENSED accusoft.com",
        "BarcodeData": [
          "C",
          "O",
          "D",
          "E",
          " ",
          "*",
          "*",
          " ",
          "U",
          "N",
          "L",
          "I",
          "C",
          "E",
          "N",
          "S",
          "E",
          "D",
          " ",
          "a",
          "c",
          "c",
          "u",
          "s",
          "o",
          "f",
          "t",
          ".",
          "c",
          "o",
          "m",
          "\u0000"
        ],
        "BarcodeDataAsByte": "Q09ERSAqKiBVTkxJQ0VOU0VEIGFjY3Vzb2Z0LmNvbQA=",
        "BarcodeName": "Code 39",
        "BarcodeType": 9,
        "ModeTransitions": [],
        "Info2D": {
          "RowsDetected": 0,
          "ColumnsDetected": 0,
          "Rows": 0,
          "Columns": 0,
          "ErrorCorrectionLevel": 0
        }
      },
      ...
    ]

For the writer samples, a file called test-barcodes.bmp will be created in
the bin/Debug folder that contains the generated barcode image.

_**NOTE:** Barcode Xpress runs in Watermark evaluation mode if started without
a license and the barcode value will be partially hidden. If you would like to
do a full-featured evaluation of the product, [contact us](mailto:info@accusoft.com)._
