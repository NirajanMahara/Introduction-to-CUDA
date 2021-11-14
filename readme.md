6CS005

High Performance Computing

Lecture 6

<hr>

# GPGPU Computing with CUDA

## What is GPGPU computing?

![image](https://user-images.githubusercontent.com/69881638/141667081-7b86c5ac-6cb7-4c10-9ef4-ced8a2b81647.png)

## Why use GPGPU computing?

![image](https://user-images.githubusercontent.com/69881638/141667098-07340235-ebd6-4b1f-a483-3dfaba66bb87.png)

## Should we all have computers like this?

![image](https://user-images.githubusercontent.com/69881638/141667108-fc74f8df-9db4-4bd9-b275-dffa3bd86489.png)

## CPU vs GPU

![image](https://user-images.githubusercontent.com/69881638/141667126-24faca8c-b061-4410-83ef-8dbdd484c21a.png)

## GPU vs GPGPU

![image](https://user-images.githubusercontent.com/69881638/141667143-8b7d6f4d-bd11-46cb-bd55-650a3cff56a8.png)

## What is CUDA?

![image](https://user-images.githubusercontent.com/69881638/141667160-4ecbb540-e61d-4a81-ba67-f196a6a99677.png)

## Prerequisites

![image](https://user-images.githubusercontent.com/69881638/141667197-55318a35-ae3f-4fe1-975d-d4df7c0aeb29.png)

## Heterogeneous Computing

![image](https://user-images.githubusercontent.com/69881638/141667205-f05e9522-0d8d-4e76-b185-67c9b0967b42.png)

## Heterogenous Computing

![image](https://user-images.githubusercontent.com/69881638/141667217-17b889c0-94c3-4052-982b-645634daaa3a.png)

## Simple Processing Flow

![image](https://user-images.githubusercontent.com/69881638/141667227-3e5ffc9b-c5da-450e-aa1b-acb5ec7fff1c.png)

## Simple Processing Flow

![image](https://user-images.githubusercontent.com/69881638/141667256-45aef26b-ff04-44a6-9342-3a3a86f29b1f.png)

## Simple Processing Flow

![image](https://user-images.githubusercontent.com/69881638/141667269-863326e1-933b-4916-978f-d39cb5e1fb07.png)

## Simple Processing Flow

![image](https://user-images.githubusercontent.com/69881638/141667305-4ce844ed-fef8-4dd7-9f01-8c9e8a0de2e0.png)

## Hello World!

![image](https://user-images.githubusercontent.com/69881638/141667355-7f5eaec9-abbb-49dc-aa77-79f3be4adf43.png)

```
int main(void) {
    printf("Hello World!\n");
    return 0;
}
```

## Hello World! with Device Code

![image](https://user-images.githubusercontent.com/69881638/141667371-148b33fb-bf9c-4a38-8523-40d0cc9f7e85.png)

```
__global__ void mykernel(void) {
}

int main(void) {
    mykernel<<<1,1>>>();
    printf("Hello World!\n");
    return 0;
}
```

## Hello World! with Device Code

![image](https://user-images.githubusercontent.com/69881638/141667402-9c849889-2d0b-4052-8240-ccb40a980fa8.png)

```
__global__ void mykernel(void) {
}

```

## Hello World! with Device Code

![image](https://user-images.githubusercontent.com/69881638/141667424-e1b1dd0e-15ca-4948-bf96-437ec8394edf.png)

```
mykernel<<<1,1>>>();
```

## Hello World! with Device Code

![image](https://user-images.githubusercontent.com/69881638/141667455-8e4cb11c-8987-456a-9f78-9cad29551045.png)


## Parallel Programming in CUDA C/C++

![image](https://user-images.githubusercontent.com/69881638/141667469-f60bf5e7-e642-4901-96ad-fd2cd64597f1.png)

## Addition on the Device

![image](https://user-images.githubusercontent.com/69881638/141667490-84ad950a-d7aa-4196-a50e-6b499f003bd6.png)

## Addition on the Device

![image](https://user-images.githubusercontent.com/69881638/141667501-5f7f2aba-1383-4d16-8659-4267068c283d.png)

## Memory Management

![image](https://user-images.githubusercontent.com/69881638/141667519-c31128c8-2748-4a37-8900-c2525217de55.png)

## Addition on the Device: `add()`

![image](https://user-images.githubusercontent.com/69881638/141667535-3e0bd5bc-9f88-4278-9049-654dd0be0ea4.png)

## Addition on the Device: `main()`

![image](https://user-images.githubusercontent.com/69881638/141667568-d9514ca5-f3dc-4077-b6f3-601140ea2118.png)

## Addition on the Device: `main()`

![image](https://user-images.githubusercontent.com/69881638/141667588-f8159dec-15b2-4854-a7f0-41d2864682b7.png)

