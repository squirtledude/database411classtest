Relational Schema:
Table-Name(Column1:Domain [PK], Column2:Domain [FK to table.column], Column3:Domain,...)

User ( 
    UserID:INT[PK]
    Password:VARCHAR(255)
    Username:VARCHAR(255) 
)

Game ( 
    GameID:INT[PK]
    Name:VARCHAR(255)
    ReleaseDate:VARCHAR(255)
    RequiredAge:INT
    GenreID:INT[FK to Genre.GenreId]
    PlatformID:INT[FK to Platform.PlatformId]
    DeveloperId:INT[FK to Developer.DevelopId]
    Rating:INT
    Price:Int 
)

Genre( 
    GenreId(PK)
    Description:VARCHAR(255) 
)

Platform( 
    PlatformId(PK)
    Description:VARCHAR(255)
)

Developer(
    DeveloperId(PK)
    Description:VARCHAR(255)
)

SearchResult( 
    ResultId:INT(PK)
    UserId:INT(FK to User.UserId)
    Games:VARCHAR(255) 
)