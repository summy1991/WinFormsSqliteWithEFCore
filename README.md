# WinFormsSqliteWithEFCore
1. Crreate winforms project
2. Install 
3. Install 
4. Install
5. Create Any Class and inherited DbContext Base Class. For Example  class name is UserContext so 
  public class UserContext: DbContext
  {
      public DbSet<UserDetails> UserDetails { get; set; }
        protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
        {
            optionsBuilder.UseSqlite(@"Data Source=Db\UserDb.sqlite");
        }
  }
