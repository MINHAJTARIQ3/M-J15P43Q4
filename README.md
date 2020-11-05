 Class Member
        Private MemberName As String
        Private MemberID As String
        Private SubscriptionPaid As Boolean
        Public Sub SetMemberName(ByVal name As String)
            MemberName = name
        End Sub
        Public Sub SetMemberID(ByVal ID_num As String)
            MemberID = ID_num
        End Sub
        Public Sub SetSubscriptionPaid(ByVal IsPaid As Boolean)
            SubscriptionPaid = IsPaid
        End Sub
    End Class
    Class JuniorMember
        Inherits Member
        Private DateOfBirth As Date
        Public Sub SetDateOfBirth(ByVal dob As Date)
            DateOfBirth = dob
        End Sub
    End Class
    Sub Main()
        Dim NewMember As New JuniorMember
        NewMember.SetMemberName("Ahmed")
        NewMember.SetMemberID("12347")
        NewMember.SetSubscriptionPaid(True)
        NewMember.SetDateOfBirth(Date.FromOADate(12 / 11 / 200))
    End Sub
End Module
