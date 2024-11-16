
graph LR
    I[Input 32x32x3] --> C1[Conv+ReLU]
    C1 --> RB1[Res Block 1]
    RB1 --> RB2[Res Block 2]
    RB2 --> RB3[Res Block 3]
    RB3 --> RB4[Res Block 4]
    RB4 --> U1[UpSample 64x64]
    U1 --> U2[UpSample 128x128]
    U2 --> O[Output 128x128x3]
